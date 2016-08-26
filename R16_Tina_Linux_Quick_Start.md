#R16 Tina Linux SDK快速指南
## 一、R16 Tina Linux SDK版本下载
### 1.下载repo：
```
$ curl https://raw.githubusercontent.com/tinalinux/repo/stable/repo > ~/bin/repo
$ chmod +x ~/bin/repo
```
将~/bin目录添加到环境变量：
```
$ export PATH=~/bin:$PATH
```
### 2.下载R16 Tina Linux SDK V2.1版本
```
$ repo init -u https://github.com/tinalinux/manifest -b r16-v2.1.y -m r16/v2.1.y.xml
$ repo sync
$ repo start r16-v2.1.y --all
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
