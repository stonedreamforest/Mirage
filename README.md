# Mirage
> 驱动已签名，由于使用泄露签名，使用前请关闭杀毒软件。



#### 说明
1. 基于intel vtx && ept 技术 
2. 不与其它反反调试插件冲突


#### 测试程序
[al-khaser](https://github.com/LordNoteworthy/al-khaser)
- [ ] IsDebuggerPresent
- [ ] CheckRemoteDebuggerPresent
- [ ] Process Environment Block (BeingDebugged)
- [ ] Process Environment Block (NtGlobalFlag)
- [ ] ProcessHeap (Flags)
- [ ] ProcessHeap (ForceFlags)
- [ ] NtQueryInformationProcess (ProcessDebugPort)
- [ ] NtQueryInformationProcess (ProcessDebugFlags)
- [ ] NtQueryInformationProcess (ProcessDebugObject)
- [ ] WudfIsAnyDebuggerPresent
- [ ] WudfIsKernelDebuggerPresent
- [ ] WudfIsUserDebuggerPresent
- [ ] NtSetInformationThread (HideThreadFromDebugger)
- [ ] NtQueryObject (ObjectTypeInformation)
- [ ] NtQueryObject (ObjectAllTypesInformation)
- [ ] CloseHanlde (NtClose) Invalide Handle
- [ ] SetHandleInformation (Protected Handle)
- [ ] UnhandledExceptionFilter
- [ ] OutputDebugString (GetLastError())
- [ ] Hardware Breakpoints (SEH / GetThreadContext)
- [ ] Software Breakpoints (INT3 / 0xCC)
- [ ] Memory Breakpoints (PAGE_GUARD)
- [ ] Interrupt 0x2d
- [ ] Interrupt 1
- [ ] Parent Process (Explorer.exe)
- [ ] SeDebugPrivilege (Csrss.exe)
- [ ] NtYieldExecution / SwitchToThread
- [ ] TLS callbacks
- [ ] Process jobs
- [ ] Memory write watching
- [ ] Page exception breakpoint detection
- [ ] API hook detection (module bounds based)

#### 系统支持
1. win7 x64
2. win10 19h1 x64




#### 使用
1. 将`Mirage.sys`、`MirageV.dp32`、`MirageV.dp32`移动到`\plugins\`目录下

![image](https://user-images.githubusercontent.com/16742566/68471575-76669280-0259-11ea-9fba-e41231e83b3c.png)

2. 菜单栏-插件-幻境-进入

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
