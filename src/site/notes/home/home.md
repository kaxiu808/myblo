---
{"dg-home":true,"dg-publish":true,"title":"🏠home","permalink":"/home/home/","tags":["gardenEntry"],"dgPassFrontmatter":true}
---





# 🏠home


## Calendar 

 
	- 每日总结复盘
## - 草稿
	-  渐进



## 来源



## 空间

### - 项目

了解什么是[[home/php\|php]]

知道什么是[[home/正则表达式\|正则表达式]]

渗透测试的[[home/常用工具\|常用工具]]

### - 领域


# 信息输入

## 灵感
   * 要想处理大量的信息，必须从逻辑上动手*
   案例  这是从xpath逻辑 里面找到的。如下：
  
   文字版
   ```python
 # hot_cities = tree.xpath('//div[@class="bottom"]/ul/li/a/text()')  
 # all_cities = tree.xpath('//div[@class="bottom"]/ul/div[2]/li/a/text()')
 
 cities = tree.xpath('//div[@class="bottom"]/ul/li/a/text() | //div[@class="bottom"]/ul/div[2]/li/a/text()')
  ```
   第一页 ：a :  //div/p/a
   第二页： a:  //p/span/div/a
   
   图片版
![与逻辑](https://gitlab.com/minika1/Pic/-/raw/main/pictures/2024/03/7_18_26_5_%E4%B8%8E%E9%80%BB%E8%BE%91.png)

如果第一页有用，第二页变动得化，至少有一个逻辑是可以用的。  它们都是对 a标签的提取。

   这里用到的是或逻辑 ， 符号为 ` | ` ,  意思是只要有一个逻辑表达式有用，都可以，上述的案例是两个逻辑都有用。  
  
  
   # 处理逻辑    用`|` 符号     
 



## 文章

 -  怎么用逆向的思维[[学习区(未掌握)/逆向js\|逆向js]]拿到想要的东西
 -  了解编程中的重要[[学习区(未掌握)/python基础\|python基础]]的知识点
 -  如何通过cmd命令操作系统，可以说，只要是鼠标点的东西，都可以用cmd(伪dos)命令操作  ==>  [[系统\|伪dos命令]]


## 书籍


## 任务管理

[清单管理](https://app.todoist.com/app/project/python-js-2327571745)



<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE5MTI5NjIyXX0=
-->