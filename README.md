# Mirage
> 驱动已签名，由于使用泄露签名，使用前请关闭杀毒软件。



#### 说明
1. 基于intel vtx && ept 技术 
2. 不与其它反反调试插件冲突


#### 测试程序
[al-khaser](https://github.com/LordNoteworthy/al-khaser)


#### 系统支持
1. win7 x64 ( *`6.1.7600`*)
2. win10 19h1 x64 (*`10.0.18362.XXXX`*)

> 注：请把你需要的系统告诉我:[issues](https://github.com/stonedreamforest/Mirage/issues) 或者给我发邮件... 如果你有我的微信也可以说... 友情通道...QAQ

> 我会在我的空闲时间支持它（拒绝支持x86内核以及xp、win8、win8.1😅

> 需要至少10个人在这里表示需要它我才会支持 不然是无意义的更新支持...

#### 调试器支持
1. 现支持[x64dbg](https://github.com/x64dbg/x64dbg)，而且会持续更新...
2. 不会支持OD
3. 计划支持windbg、[cutter](https://github.com/radareorg/cutter)、[ghidra](https://github.com/NationalSecurityAgency/ghidra) 。后俩者需要它们本身先支持调试功能


#### 技术支持(包括但不限于反反调试、驱动读写、驱动注入...
> 如果你要支持某一特定程序或系统, 请邮件联系我，我将成为你的私人技术支持... （*很明显这将是付费的.*



#### 使用
0. 使用[`PDBDownloader.exe`](https://github.com/rajkumar-rangaraj/PDB-Downloader)下载`ntoskrnl.exe`文件 (默认在下载在C盘

![image](https://user-images.githubusercontent.com/16742566/68540402-a6827280-03cc-11ea-9e5e-b54916db71f5.png)

1. 使用`MVConfigBuild.exe`生成`config.mv`配置文件 并将之移动到c盘根目录`C:\`
> MVConfigBuild.exe `C:\symbols\ntkrnlmp.pdb\hashxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\ntkrnlmp.pdb`
![image](https://user-images.githubusercontent.com/16742566/68540440-0da02700-03cd-11ea-9810-4bda0d9e1c18.png)


2. 将`Mirage.sys`、`MirageV.dp32`、`MirageV.dp64`移动到`\plugins\`目录下

![image](https://user-images.githubusercontent.com/16742566/68471575-76669280-0259-11ea-9fba-e41231e83b3c.png)

3. 菜单栏-插件-幻境-进入

![image](https://user-images.githubusercontent.com/16742566/68471759-d5c4a280-0259-11ea-8922-46569af7d9be.png)


- 附加
> 输入进程id - 点击`附加进程` - 点击`开启`

![image](https://user-images.githubusercontent.com/16742566/68471844-06a4d780-025a-11ea-9c12-0c07e11b53d5.png)


- 启动调试
> 直接点击开启

![image](https://user-images.githubusercontent.com/16742566/68471860-13293000-025a-11ea-8319-1707dcb9a0d2.png)


#### 演示
![Bn2pqgw32f](https://user-images.githubusercontent.com/16742566/68470102-5e414400-0256-11ea-8f85-aa0e893f71ea.gif)



#### 当前版本
[v20191108](https://github.com/stonedreamforest/Mirage/releases/tag/v20191108)

#### 最新版
[最新版](https://github.com/stonedreamforest/Mirage/releases)


#### 更新日志
[CHANGELOG](https://github.com/stonedreamforest/Mirage/blob/master/CHANGELOG.MD)



## 最后
未来的某一天会公开代码... 

