# 个人Linux笔记
***

## 1)用户帐号	
### ‘$’表示普通用户
### ‘#’表示超级管理员
## 2）脚本执行
### 一种是将脚步作为sh的命令参数
### 另外一种是将脚步作为具有执行权限的可执行文件
####***在Bash中，每一个命令序列是通过使用分号或换好符来分割的
## 3) 注释
### 字符‘#’指明注视的开始。注释部分以‘#’开始，一直延续到行尾
## 4）echo命令
### echo是用于终端打印的命令，默认情况下每次调用后会添加一个换行符
###例子：
####echo "hello world"->hello world
####echo hello world ->hello world
####echo 'hello world' ->hello world
####说明：
##### 双引号支持普通文本和变量输出
###### var="hello";echo "$var world;java"->hello world;java
##### 单引号原样输出，不支持变量
###### var="hello";echo '$var world;java'->$var world;java
##### 不带引号支持普通文本和变量输出，带分号出错问题
###### var="hello";echo $var world->hello world
###### var="hello";echo $var world;test->hello worl;-bash: javad: command not found(出错)
##### -n参数 
###### 忽略echo输出的换行符
##### 颜色输出 \e[0;31m(文本颜色) xxxxxxx \e[0m（颜色恢复）  
###### echo -e "\e[0;31m this is read \e[0m"->this is read（文本红色）
## 5）printf命令
###printf "%-5s %-10s %-5s\n"   no name remark
###printf "%-5s %-10s %-4.2f\n" 1  tom    98.123
###printf "%-5s %-10s %-4.2f\n" 2  jack   123.123
### 输出：
### no    name       remark
### 1     tom        98.12
### 2     jack       123.12
### 说明：替换符
###### %s  字符串 %-5s  
###### %d  数字   %-5d  
###### %f  浮点   %-4.2f .2保留2位小数
###### -   左对齐  







