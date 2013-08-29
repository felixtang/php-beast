  _____  _    _ _____    ____  ______           _____ _______ 
 |  __ \| |  | |  __ \  |  _ \|  ____|   /\    / ____|__   __|
 | |__) | |__| | |__) | | |_) | |__     /  \  | (___    | |   
 |  ___/|  __  |  ___/  |  _ <|  __|   / /\ \  \___ \   | |   
 | |    | |  | | |      | |_) | |____ / ____ \ ____) |  | |   
 |_|    |_|  |_|_|      |____/|______/_/    \_\_____/   |_|   
==============================================================

此模块可以用于商业,
使用DES加密算法加密,
版权归原作者.


使用方法:
=========
修改beast.c文件的authkey加密key, 编译安装,
接着使用beast_encode_file()函数进行加密,
加密后的文件beast模块能自动识别.


编译安装如下:
-------------
$ wget https://github.com/liexusong/php-beast/archive/master.zip
$ unzip master.zip
$ cd php-beast-master
$ phpize
$ ./configure
$ sudo make && make install

编译好之后修改php.ini配置文件, 加入配置项: extension=beast.so, 重启php-fpm

+---------------------------------------------+
|  温馨提示: 1) 缓存设置越大, 效率越高        |
|            2) 可以修改key.c文件中的加密key  |
+---------------------------------------------+


配置项:
+---------------------------------------------+
| beast.cache_size = size                     |
| beast.log_file = "path_to_log"              |
| beast.lock_path = "path_to_locker"          |
+---------------------------------------------+

TODO:
-----
* 增加opcode缓存

------------------------------
作者: 列旭松(280259971@qq.com)

我的著作: http://book.jd.com/11123177.html
我的团队: 280259971
定制版本请联系: 280259971
捐赠:  <a href='http://me.alipay.com/liexusong'> <img src='https://img.alipay.com/sys/personalprod/style/mc/btn-index.png' /> </a>
------------------------------
