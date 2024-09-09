# 项目介绍
&nbsp;&nbsp;&nbsp;&nbsp;This is a VSCode plugin used to automatically generate code snippets related to Linux C programming.
# 代码片段介绍
## 头文件代码块
### 前缀介绍
|前缀|作用|其它|
|--------|----------|----------|
|**lch**|头文件模板 ,如<br> `#ifndef _XXX_H_ ` <br> `#define _XXX_H_ `<br> `/* code */`  <br>` #endif`| 无
|**lcfh**|在xxc中加入 `#include "xx.h"` 头文件引用| 无
|**#i**|在文件中加入 `#include ".h"` 头文件引用| 无
|**#i<**|在文件中加入 `#include <.h>` 头文件引用| 无
|**#string**|在文件中加入 `#include <string.h>` 头文件引用| 无
|**#std**|在文件中加入 `#include <stdio.h>` <br> ` #include <stdlib.h>` 头文件引用| 无
|**#err**|在文件中加入 `#include <errno.h>` <br> ` ` 头文件引用| 无
|**#opendir**|在文件中加入 `#include <sys/types.h>` <br>  ` #include <dirent.h>` 头文件引用| 无


## 目录代码块
### 前缀介绍
|前缀|作用|其它|
|------|------|-----|
|**lcdir_foreach**|通过`opendir()` `readir()` 来遍历目录,只遍历单层目录(**注意!!**` readir()`为非线程安全函数,请谨慎使用).|无|
|**lcdir_filter_notdir**|通过`opendir()` `readir()` 来遍历目录下的非目录文件,只遍历单层目录(**注意!!**` readir()`为非线程安全函数,请谨慎使用).|无|
|**lcdir_filter_dir**|通过`opendir()` `readir()` 来过滤出目录下的目录,只遍历单层目录(**注意!!**` readir()`为非线程安全函数,请谨慎使用).|无|
|**lcdir_filter_cb**|通过`opendir()` `readir()` 来过滤出目录下的字符或块文件,只遍历单层目录(**注意!!**` readir()`为非线程安全函数,请谨慎使用).|无|
|**lcdir_filter_rl**|通过`opendir()` `readir()` 来过滤出目录下的普通或链接文件,只遍历单层目录(**注意!!**` readir()`为非线程安全函数,请谨慎使用).|无|
|**lcdir_filter_sp**|通过`opendir()` `readir()` 来过滤出目录下的socket或管道文件,只遍历单层目录(**注意!!**` readir()`为非线程安全函数,请谨慎使用).|无|

## 字符串代码块
### 前缀介绍
|前缀|作用|其它|
|------|------|-----|
|**lcstr_h**|加入目录相关的头文件<br> `#include <string.h>` |无|
|**lcstr_split_foreach**|通过strtok_r()分隔符将字符串分割后，遍历出所有分割后的子串(**注意!!**` 此操作会修改原字符串内容)。 |无|




