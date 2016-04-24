---
layout: post
title: "學習紀錄一"
date: 2016-04-24 13:57:25 +0800
comments: true
categories: learningrecord
---



##Ruby

###<mark>.underscore 

```
'ActiveModel'.underscore         # => "active_model"

'ActiveModel::Errors'.underscore # => "active_model/errors"
```

對 **string** 使用

用於切換 檔名  與路徑  

###<mark>.fetch

```
h = { "a" => 100, "b" => 200 }
h.fetch("a")                            #=> 100
h.fetch("z", "go fish")                 #=> "go fish"

h.fetch("z") { |el| "go fish, #{el}"}   #=> "go fish, z"
```
對 **hash** 使用

抓出hash裡面的值  如果沒有就報錯   如果沒有但有給default 
回報default 的值
如果沒有 但有定義後面的 code block 把搜尋的值 塞進去




##Factroyfirl

###<mark>sequence

```
FactoryGirl.define do
  sequence :email do |n|
    "person#{n}@example.com"
  end
end
```

用於產生序列化的變數
使用上要好於使用隨機數字-> 不會重複



