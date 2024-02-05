---
{"dg-home":true,"dg-publish":true,"permalink":"/php1/","tags":["gardenEntry"],"dgPassFrontmatter":true}
---



# 了解php

## 章节1： 了解PHP

php 是什么
php 能干什么？ 开发网站
输出一个属于自己的第一个php程序
```php
<?php 
echo 'Helo world'>;
?>
```

<?php ?>  标识 [告诉你]
echo  'hello world';   代码

echo  [指令] 输出

echo  ’echo‘;          字符串无实际意义，只是被当作文本输出

CD光盘

## 章节2： 人人都会编程


起床上班

打招呼 if  判断[需要预先设定]

```php
<?php 
$sex ='男'；  // 变量 注释
if ($sex == '男'){  //如果
echo '帅哥，进店里来看看把，有XXXX'；}
else {echo "妹妹我们店有xxxx化妆品"；}
?>
// 变量 运算 控制
变量 比较运算 分支语句
```

## 章节3:  变量就是一个盒子

```php
变量教学 - 变量就是一个盒子 
计算机特点：运算飞快，忘的也飞快
变量就是个盒子储存东西的
$age = 18;
$age = 19;
echo $age;
$age = $age + 1 //赋值
$age = 20
变量命名名字

必须是字母[a-zA-Z]、下划线、数字[0-9]名字，不能数字开头
$age =1;
$_=123;
//$!=321; 
```

## 章节3： 运算符

加减乘除   取余 比较  大小等于    小于等于  不等于

```php
1+1
$wang = 100000;
$Ma =  150000;
echo $Ma + $wang
$A1 = 45;
$A = $A1*15;
echo $A

取余：3/2= 1.5 取整数能运算余数下树
7/3 = 3*2 = 6 取余1

echo 7%3

$Fang = 18;
$Zheng = 19;
if ($Fan>15){
echo '方先生大于15岁'；
}
else{echo '方先生不大于15岁'}
<?php

?>
```


## 章节5：控制结构介绍


顺序结构  分支语句   循环语句

穿衣服  穿鞋子  刷牙洗脸 

```php
$a = 1;
$a = 2;

分支语句  [选择]
$sex = '男生'；
if($sex =='男生')
{echo 'hello Boy';}
else
{echo 'Hello gril';}

循环语句 
while ()  不断的做某件事

比如说我们现在在喝水

<?php
$water = 1;
while ($water<6){
echo '我喝了'.$water.'杯，服务员再给我杯水吧<br/>
';
$Water =$water +1;
}
echo '谢谢，我喝了'.$water.'杯水，不渴了'；
?>
```

## 章节6 ：你已经学会编程

```
打印1-100
打印1-100偶数   //偶数的定义  能被2整除
遇到7的倍数  打印字符A
遇到13 的倍数 打印字符B

echo ’1‘；
echo ’2‘；

------
echo '100'；

变量 循环 运算
```

```php
<?php 
$i = 1;
while($i<=100){
	if ($i%2 == 0){
	echo $i."<br />";
	}
	$i =$i+1;
}
?>

<?php

$i = 1;
while($i<=100){
	if ($i%7 == 0){
		echo "A<br />";
}
	else{if ($i%13 ==0){
		echo "B<br/>";
	}else{echo $i."<br/>";}
	}
	
	$i =$i+1;
}
?>
```


## 章节7 字符串的处理函数

7.字符串的处理
1.字符串是什么   // 字符串其实就是文本是记录 ，跟字符串对立的就是代码
2.单双引号的区别

>"$代码"  '文本'

```php
<?php
$a = 'b'
$b = "$a";
echo $b;
?>
```

>3.字符串处理函数

>strstr ()   字符串的匹配和寻找

```php
案例
<?php 
$a = 'xxxx,hello';
if (strstr($a,'CNM')=='CNM'){
	echo 'No';
}
else{
	echo "ok";
}

?>
```

>str_replace('要替换的东西','替换成什么','在那个语句替换')    

```php
案例 

echo str_replace("world","shanghai","hello world!")."<br/>";
echo str_replace("Wang","Li","hello Wang");
```

```php
<?php   
$a = 'admin\'';
echo $a;  
?>

admin\


<?php   
$a = "admin\\";
echo $a;  
?>

admin\ \\
```
## 章节8 数组讲解

数组
实际上是一排柜子
存东西
号码牌  标识

号码牌 key键 [独一无二的不会重复]

key 键 value值

```php
<?php   
$a = array('001'=> '70帽子','002'=>'ssg衣服','003'=>'nf的手机');
$b =1;
var_dump($b);  
?>

<?php   
$a = array(001=> '70帽子','vip'=>'ssg衣服','003'=>'nf的手机');
echo $a['vip'];
 
?>
<?php
// 定义了数组
// 取出了东西
var_dump($a)
?>
```

## 终章9：php 接受传参

制作一个网页

> 如何获取GET|POST传参

```php
GET 传参 POST传参 
<?php
var_dump($_GET)
?>
```

```php
<?php
if ($_GET['fengshu']<60){
	echo '同学你考试不及格';
}
else{
	echo '同学你及格了';
}

?>
```
如下图[传参](https://github.com/kaxiu808/xuebiji/blob/main/img/%E4%BC%A0%E5%8F%82.png)

>传参不能一个一个的去输入，这才有了表单

什么是表单？
表单在网页中主要负责数据采集功能。
一个表单有三个基本组成部分：
表单标签：这里面包含了处理表单数据所用动态脚本的URL以及数据提交到服务器的方法。
表单域：包含了文本框、密码框、隐藏域、多行文本框、复选框、单选框、下拉选择框和文件上传框等。
表单按钮：包括提交按钮、复位按钮和一般按钮；用于将数据传送到服务器上的动态脚本或者取消输入，
还可以用表单按钮来控制其他定义了处理脚本的处理工作。
```php

表单标签：
<form action= "URL" method="GET/POST" >
表单域：即表单组件，主要有
文本框、密码框、隐藏域、复选框、单选框、文件上传框
多行文本框（文本域）
下拉选择框
表单按钮：
提交按钮
复位按钮
一般按钮
```

创建一个名为1.html文件
```html
<form action ='18.php' method="POST">
<input type='text' name='fenshu'/><br/>
<input type='submit' value= "提交"/>
</form>
```
[表单域](https://github.com/kaxiu808/xuebiji/blob/main/img/%E8%A1%A8%E5%8D%95%E5%9F%9F.png)

```php
$_REQUEST 是都可以传$_GET 和 $_POST
```

创建一个名为18.php文件代码如下：
```php
<?php
$fenshu =$_REQUEST['fenshu'];
if($fenshu>= 60){
	echo '及格';
}
else{
	echo '不及格';
}
?>
```

# 10.初识数据库

数据库是什么？  // 数据 仓库
它的结构是怎么样的？ // 库 表 字段 记录
常见的数据库有哪些？ // MYsql   MSSQL


数据库他是靠SQL语句

x张表变成一个库

## 1.数据库结构的改变


知道自己现在自己数据库有什么结构。

	show databases  查看有什么库

	show tables   查看有什么表

	use 库名  [进入库]

	desc 表名  查看表的结构


>改变自己数据库结构

	建立数据库： Create database 库名

	删除数据库：Drop database 库名

	建立表：create table 表名(字段名 字段类型，字段名2，字段类型)

出现了不知道的东西，字段类型是什么？
就是字段的格式，例如int数字 [只能存储数字]

varchar 字符串 [能存储字符串]   varchar(255)   [能存储255个字符]



>创建表

	create table ssg(id int(8),name varchar(255));

	删除数据表 ：Drop table 表名

添加表里面的字段：

	Alter table 表名 add 字段名  字段类型

删除表里面的字段：

	Alter table 表名 drop 字段名

修改表内字段名；
	alter table 表名 change 旧字段名  新字段名 新类型；
	

查看有什么数据库 、表
使用库
查看表结构
建立库、表
删除库、表
修改表里面的字段 [增 删 改 ]

## 第三节 数据库的增删改查

增删改查 对记录

插入数据
查询数据
修改数据
删除数据

英文分号结尾，代码部分大小写不敏感，但是数据敏感

database()

>插入数据(增)：

	insert into 表名 values (值，值)

	insert into 表名（列名1，列名2）  values(值1，值2)

>查询语句：

	select  * from 表名 where 条件

 `*是字段名` 
 
	select  字段名 from 表名 where 条件

>修改数据：

	update 表名 set 列名 = 新列值 where 列名 = 旧列值

	update 表名 set 列名 = 新列值，列名2 = 新列值 where 列名 = 旧列值
	
update ssg set username=999,password='SF' where username =999;
>删除数据

	Delete from 表 where 列名=列值

## 第四节 运算符和处理结果

>结果排序

	order by 1 排序第一个字段

	order by 字段名 排序写了字段名的这个字段

		默认升序 [asc]
		降序 [desc]
		select * from ssg order by 1 desc;

>分页

	limit n,m
			limit 从那里开始，取多少行数据

>多行数据一起输出

	group_concat()

>模糊查询：

	like %a%    查询包含a的所有值
	like a%     查询a开头的所有值
	like %a     查询a结尾的所有值

>休眠函数

	sleep(2)     服务器进入摸鱼模式，故意拖2秒返回数据

>查询当前所在库

	select database();

>查询当前所在表

	show tables；


select * from ssg where password like '%a%';


### 处理结果 

数学运算符号：

	+ - * / %

   他和PHP中没有啥区别

逻辑运算符：

and    [满足两个条件才可以]  既要这要，又要那样

or      [满足一个条件就可以]   这个或那个都行

not    [取反]    大小姐发脾气了，我要去，她非要留。非要和我做对


## 第五节 子查询和联合查询

联合查询和子查询

>联合查询： 

	union  将两个查询语句的结果一起输出 [重复的不输出] 
	union  all  将两个查询语句的结果一起输出 [重复也输出]
	需要满足条件，相同列数

>子查询: 在原本的SQL语句中写小括号，优先执行一个查询语句

	select * from ssg where password = (select uname from nf where id=1);  => select * from ssg where password =10


## 第六节 php 与数据交互

正常网站：

		传参 -> php 处理 -> 去数据库存东西获取东西 -> 显示数据

这里有很核心的一步是php能够操作数据库，这里就需要用到php的mysqli扩展

   这个扩展时操作mysql数据库，自带的，你可以理解为他是一些函数，当你看到一个函数时mysqli_的适合一般都属于mysqli扩展。

  mysqli扩展的核心就是PHP去操作数据库


### 如何操作

     建立连接：
```php

mysqli_connect (链接地址，账号，密码，库名) =>  $conn =mysql_connect('localhost','root','root','fuli');

mysqli_select_db(连接，库名)
	mysqli_select_db($conn,'fuli');
mysqli_query(连接，执行SQL语句)
	$sql = insert into nf value(88,'PHP');
	mysqli_query($conn.$sql);

```

### 第二节 编写一个属于你的网站

上节课讲了操作数据库语句，但是很多适合我们需要取出内容，如何输出？

```php
$result = mysqli_query($conn,$sql);
mysqli_fetch_array($result);
```
     将数据库执行的结果转换为数组

创建后台管理数据
```php
<meta setchar='UTF-8'/>
后台管理
<form action='3.php' method='POST'>
帐号<input type='text' name='username' /><br/>
密码<input type='text' name='password' /><br/>
<input type='submit' value='提交'>	
</form>	
```
创建2.php连接数据库
```php
<?php
$conn = mysqli_connect('localhost','root','root','fuli');
$sql = "select*from fenshu where ig=1";
$result = mysqli_query($conn,$sql);
while ($a = mysqli_fetch_array($result)){
	echo $a['name'].' ';
	echo $a['fs'].' ';
	if($a['ig'] == 1){
		echo 'Yes<br />';
	}
	else{
		echo 'NO<br />';
	}
}

?>
```

创建一个名为3.php 登录

```php
<meta setchar='UTF-8'/>
<?php
$username = $_POST['username'];
$password = $_POST['password'];
$conn = mysqli_connect('localhost','root','root','fuli');
$sql = "select*from admin where username='$username' and password='$password'";
$result = mysqli_query($conn,$sql);
if (mysqli_fetch_array($result)['username'] == 
	$username){echo '登陆成功';}
else{
	echo '登陆失败';}

?>
```

## 后端基础PHP-表单验证


一、什么是表单？

二、如何创建一个表单

三、接收并验证表单

四、PHP和数据库交互


表单验证：php + 数据库 + 前端


PHP的文件，一定要放在网站根目录，而且后缀名，正常情况下必须是PHP

PHP文件：可以混写，写PHP也可以写HTML

```php
echo 1;
<?php
echo 1;


<meta charset='UTF-8'>  HTML代码，指定了编码格式
	聂凤666
<?php echo "聂凤666"?>


?>
```

表单在网页中主要负责数据采集功能。 [框] （和网站交互）
什么东西会有数据采集的功能？

注册、登录、个人信息、搜索资料

世界上没有无缘无故的爱也没有无缘无故的恨
凡事皆有因果：渗透测试
[你因为输入了恶意的数据，所以网站被你黑了]

表单的组成：

	 表单标签：告诉别人我这里是一个表单[数据该传到哪里、该用什么方式]
	表单域：形形色色的框
	 表单按钮：告诉别人我填完了

```<form action="1.html" method="get">

<form>
         action 数据传到那里
         method  改用什么方式传(GET/POST)
</from>

GET 传参速度更快，但是会在网址(url)中显示

POST  没有长度限制、数据不会在URL显示

<form action="https://www.baidu.com/s" method="get">
	<input type='text' name ='wd'/>
	<input type='text' name ='nf'/>	
	<input type='Submit'/>
	
</form>

from 数据库
form 表单

计算机中：PHP中，后端 [存在变量的概念 $a=1]

= 赋值 $a =1;
== 比较 $a ==2; 比较的是数值 2 ==2
=== 完全比较 比较数字和类型

	1  2  3 数字类型
	a b c   字符类型
	' '、 " "  引号内的都是字符串(不是代码不是数字)
		 单引号不会对变量进行解析  [引号外的全是代码]
		 双引号会对变量进行解析

登录框要做到多用户登录(数据库)

	数据的仓库
			库：多个表在一起就是库
			表：xls表格
			字段：列 表头
			数据(行)：最终的内容。密码是123456

select 字段名 from 表名 where 条件    查询语句的基础

	insert   插入数据    注册是在干什么？
	delete  删除数据    注销用户
	update  更改数据    修改个人资料


数据库的基础、核心(增、删、改、查)


select 字段名

	数据库不存在变量的概念，数据库属于SQL语言 。他没有变量。

 = 比较
 select * from admin where username = 'admin' and assword ='123456'


```