#R40 Tina Linux SDK快速指南
## 一、R40 Tina Linux SDK版本下载
### 1.下载repo：
```
$ curl https://raw.githubusercontent.com/tinalinux/repo/stable/repo > ~/bin/repo
$ chmod +x ~/bin/repo
```
将~/bin目录添加到环境变量：
```
$ export PATH=~/bin:$PATH
```
### 2.下载R40 Tina Linux SDK V1.0版本
```
$ repo init -u https://github.com/tinalinux/manifest -b r40-v1.y -m r40/v1.y.xml
$ repo sync
$ repo start r40-v1.y --all
```
##二、R16 Tina Linux SDK V2.1版本编译
```
$ source build/envsetup.sh
$ lunch astar_parrot-tina
$ make -j
$ pack [-d]
```
##三、固件烧写
###Windows刷机工具phoenixsuit
工具位于 tools/aw_tools

###ubuntu刷机工具LiveSuit
工具位于 tools/aw_tools
注：R40 Tina Linux SDK V1.0版本基于Tina Linux V2.1版本构建
