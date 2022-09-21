# CRC32-Tools_整合版
## 一款CTFer专属的CRC碰撞全自动化脚本（单脚本整合版）
## 1#关于该项目
在我们日常的CTF比赛中，通常会遇到压缩包破解的问题。其中重要的一个操作就是通过CRC碰撞来获取压缩包内小文件的内容，从而尝试解密压缩包
而我在实际的CTF比赛中，发现常用的CRC的爆破脚本并不好用（主要是还需要一些人工操作，如果压缩包内的文件较多，非常麻烦），就萌生了自己写一个自动化CRC碰撞脚本出来的想法

本项目的特点：
- 适配性高，能方便运行于Python3环境
- 操作简单，适合CTFer上手，可自动化通过CRC碰撞获取内容
- 傻瓜式操作，只需要输入同目录下的压缩包文件名即可
- 更新了整合版，支持Tab补全文件名，更加方便操作

## 2#使用方式
在大部分的CTF比赛中，考题一般都会考察内容为1Byte/2Byte/3Byte/4Byte的CRC碰撞，所以目前我就写了这四个版本，如果后面有需求，我会优化或者写其他的版本

**使用场景：当你拿到一道压缩包题目，发现压缩包内有多个同样大小的小文件，基本就可以确定为CRC碰撞了**
![DemoZip](./DemoZip.png)
**根据压缩包内文件的大小，选用本脚本的-4参数进行运行即可**

本项目主要由1个Python脚本构成（需要Python3环境运行脚本）：
- /SingleFile_Version：单文件版本，各个模块分离出来使用
- CRC32-Tools.py：单脚本整合版，直接使用参数即可

使用截图如下：
![Demo](./Demo-4Byte.png)
**如果各位师傅觉得这个工具好用，麻烦给个Star，万分感谢！！！**

## 3#注明
- 本项目仅用作CTF学习交流，本人一概不负任何责任
- 这是我参加某次比赛时候，遇到CRC碰撞题目临时做的脚本，本身并没有做多线程或者优化，碰撞速度并不是很快（后面版本考虑优化速度）
- 本人CTF实力挺菜的（真的），所以别找我帮你们看题目，哈哈
- 感谢各位师傅的关注和支持，对本项目的Demo.zip解密有惊喜哦，哈哈
- **如果各位师傅觉得这个工具好用，麻烦给个Star，万分感谢！！！**
- 如果在使用过程中有问题，欢迎各位师傅提issues给我哈
