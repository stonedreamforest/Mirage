![Mirage](https://img.shields.io/github/tag/stonedreamforest/Mirage?style=flat-square)
![Mirage](https://img.shields.io/github/release/stonedreamforest/Mirage/all.svg?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues-raw/stonedreamforest/mirage?style=flat-square)
![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/stonedreamforest/mirage?style=flat-square)
![GitHub Releases](https://img.shields.io/github/downloads/stonedreamforest/Mirage/latest/total?style=flat-square&logo=github)
![GitHub All Releases](https://img.shields.io/github/downloads/stonedreamforest/Mirage/total?label=downloads-total&logo=github&style=flat-square)
[![HitCount](http://hits.dwyl.io/stonedreamforest/Mirage.svg)](http://hits.dwyl.io/stonedreamforest/Mirage)


# Mirage
> 驱动已签名，由于使用泄露签名，使用前请关闭杀毒软件。




#### 说明
1. 基于intel vtx && ept 技术 
2. 不与其它反反调试插件冲突


#### 功能支持

- [x] IsDebuggerPresent
- [x] CheckRemoteDebuggerPresent
- [x] Process Environment Block (BeingDebugged)
- [x] Process Environment Block (NtGlobalFlag)
- [x] ProcessHeap (Flags)
- [x] ProcessHeap (ForceFlags)
- [x] NtQueryInformationProcess (ProcessDebugPort)
- [x] NtQueryInformationProcess (ProcessDebugFlags)
- [x] NtQueryInformationProcess (ProcessDebugObject)
- [x] NtSetInformationThread (HideThreadFromDebugger)
- [x] NtQueryObject (ObjectTypeInformation)
- [x] NtQueryObject (ObjectAllTypesInformation)
- [x] CloseHanlde (NtClose) Invalide Handle
- [x] SetHandleInformation (Protected Handle)
- [x] Hardware Breakpoints (SEH / GetThreadContext)
- [x] NtYieldExecution / SwitchToThread
- [x] Process jobs
- [x] Memory write watching
> 仅聚焦内核模式能处理的检测功能 （如有遗漏或你有任何想法、建议请告诉我

测试程序：[al-khaser](https://github.com/LordNoteworthy/al-khaser)

#### 系统支持
1. win7 x64 ( *`6.1.7600`*)
2. win10 19h1 x64 (*`10.0.18362.XXXX`*)


#### 调试器支持
1. 现支持[x64dbg](https://github.com/x64dbg/x64dbg)，而且会持续更新...
2. 不会支持OD    [支持OD？点击回复投票](https://github.com/stonedreamforest/Mirage/issues/4)
3. 计划支持~~已支持windbg~~、[cutter](https://github.com/radareorg/cutter)、[ghidra](https://github.com/NationalSecurityAgency/ghidra) 。后俩者需要它们本身先支持调试功能


#### 使用
0. 使用[`PDBDownloader.exe`](https://github.com/rajkumar-rangaraj/PDB-Downloader)下载`ntoskrnl.exe`的`pdb`文件 (默认在下载在C盘

![image](https://user-images.githubusercontent.com/16742566/68540402-a6827280-03cc-11ea-9e5e-b54916db71f5.png)

------------------------------------------


1. 使用`MVConfigBuild.exe ntoskrnl.pdb`生成`config.mv`配置文件 并将之移动到c盘根目录`C:\`

*管理员启动CMD*:

> MVConfigBuild.exe `C:\symbols\ntkrnlmp.pdb\hashxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\ntkrnlmp.pdb` (你应该确保`MVConfigBuild.exe` 和`msdia140.dll`在同一目录下

![image](https://user-images.githubusercontent.com/16742566/68540440-0da02700-03cd-11ea-9810-4bda0d9e1c18.png)

*可用离线版：[离线版config](https://github.com/stonedreamforest/Mirage/tree/master/config) （每个人都可以上传相应版本配置到此仓库.*

*格式：[版本.mv] 比如 ：**10.0.18362.295.mv**（可以使用cmd查看*

![image](https://user-images.githubusercontent.com/16742566/68569294-b9627900-0498-11ea-90c1-35d2f3af2ad6.png)


------------------------------------------



2. 文件放置
    + x64dbg：
    > 将`MirageV.dp32`、`MirageV.dp64`移动到对应`\plugins\`目录下
    ![image](https://user-images.githubusercontent.com/16742566/68994420-b4009680-08bd-11ea-8a21-43a52dd789a9.png)
    
    1. 运行：菜单栏-插件-幻境-进入
    
    ![image](https://user-images.githubusercontent.com/16742566/68471759-d5c4a280-0259-11ea-8922-46569af7d9be.png)
    
    + windbg：
    > 将`MirageV.dll`移动到对应`\Debuggers\bit??\`目录下
    ![image](https://user-images.githubusercontent.com/16742566/70392479-7a81fd80-1a1b-11ea-86ed-6af8d0ab5379.png)
    
    1. 运行：`windbg -a MirageV.dll `
    2. 再次运行：`!MirageVRun`
    
    
    + 驱动：
    > 将`Mirage.sys`移动到`C:\Windows\System32\drivers\`目录下
    ![image](https://user-images.githubusercontent.com/16742566/68994431-d5618280-08bd-11ea-88f8-63cbf0bec16a.png)

------------------------------------------


3. 使用

- 附加
> 输入进程id - 点击`附加进程` - 点击`开启`

![image](https://user-images.githubusercontent.com/16742566/68471844-06a4d780-025a-11ea-9c12-0c07e11b53d5.png)


- 启动调试
> 直接点击开启

![image](https://user-images.githubusercontent.com/16742566/68471860-13293000-025a-11ea-8319-1707dcb9a0d2.png)


#### 演示
![Bn2pqgw32f](https://user-images.githubusercontent.com/16742566/68470102-5e414400-0256-11ea-8f85-aa0e893f71ea.gif)



#### 当前版本
[v20200224](https://github.com/stonedreamforest/Mirage/releases/tag/v20200224)

#### [点击查看：历史版本及最新版](https://github.com/stonedreamforest/Mirage/releases)


#### 更新日志
[CHANGELOG](https://github.com/stonedreamforest/Mirage/blob/master/CHANGELOG.MD)

#### 相关
- [Navy: 轻量级自动分析病毒程序调用上下文、游戏反调试实现技术...](https://github.com/stonedreamforest/Navy_public)

## 最后
未来的某一天会公开代码... 

