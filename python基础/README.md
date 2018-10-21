# python基础

## python:一种解释型、面向对象、动态数据类型的高级程序设计语言

### 特点

1. 易于学习、阅读、维护
2. 丰富的第三方扩展库
3. 可移植，支持多种操作系统
4. 可扩展，兼容C代码

**缺点**

1. 运行速度慢：解释型语言，每次都要先编译再运行
2. 代码不能加密

数据存储单位：

```
8 bit == 1 Byte 一字节
1024 B == 1 KB （KiloByte） 千字节
1024 KB == 1 MB （MegaByte） 兆字节
1024 MB == 1 GB （GigaByte） 吉字节
1024 GB == 1 TB （TeraByte） 太字节
1024 TB == 1 PB （PetaByte） 拍字节
1024 PB == 1 EB （ExaByte） 艾字节
1024 EB == 1 ZB （ZetaByte） 皆字节
1024 ZB == 1 YB （YottaByte） 佑字节
1024 YB == 1BB（Brontobyte）珀字节
1024 BB == 1 NB （NonaByte） 诺字节
1024 NB == 1 DB （DoggaByte）刀字节
```

## pip管理扩展库
1、常用命令

```
pip download package[==version]
pip freeze [> requirements.txt]
pip list
pip install package[==version]
pip install package.whl 
pip install -r requirements.txt
pip install --upgrade package
pip uninstall package[==version]
```
2、使用配置文件配置更改下载源

```
[global]
trusted-host=mirrors.aliyun.com
index-url=http://mirrors.aliyun.com/pypi/simple/
```
配置文件放置位置

```
Linux下: ~/.pip/pip.conf
windows下:用户文件夹下\pip\pip.ini
```

3、使用命令行临时改变pip源

```
pip install -i <mirror> --trusted-host <mirrorhost> package
例如
pip install -i http://pypi.douban.com/simple/  --trusted-host pypi.douban.com  pandas
```
国内源:

* http://pypi.v2ex.com/simple/
* http://pypi.douban.com/simple/
* http://mirrors.aliyun.com/pypi/simple/
