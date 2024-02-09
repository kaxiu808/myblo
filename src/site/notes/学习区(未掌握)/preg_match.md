---
{"dg-publish":true,"permalink":"/学习区(未掌握)/preg_match/","dgPassFrontmatter":true}
---

一、 preg_match()函数的定义

preg_match()函数是PHP中用于匹配正则表达式的函数之一。该函数用来检索字符串中是否存在符合正则表达式模式的子字符串，并将结果存储在一个数组中，返回值是匹配成功的次数。函数定义如下：

`preg_match(pattern, subject, matches)` 

pattern：正则表达式模式，如'/^[a-zA-Z0-9_]+$/'。
subject：要匹配的字符串，如'hello world'。
matches：存储匹配结果的数组，可以省略不写，也可以在函数外先定义后写入。
{ #ba8839}


`preg_match("/zkaq.*key.{2,9}:\/.*\/(key*key)/i", trim($_GET["id"]), $match)

. 任意字符
`*0次或者多次
.{2,9} 任意字符两次到九次
zkaqaakeyabca:/add/keykeykey

key*
y*
(key)*

trim 函数是移除字符串两侧空白字符或者其它预定义字符。  就是去空格。

