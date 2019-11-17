
#### 2019-11-17
0. [修复错误提示在非中文系统乱码的问题 issues/6](https://github.com/stonedreamforest/Mirage/issues/6)

#### 2019-11-16
0. 修复[issues/5](https://github.com/stonedreamforest/Mirage/issues/5)
1. 将`Mirage.sys`的默认目录设为`C:\Windows\System32\drivers\`目录下 避免创建多个副本
2. 一些bug修复

#### 2019-11-11
0. 修复[issues 2](https://github.com/stonedreamforest/Mirage/issues/2)
1. 添加`config`离线文件 可以根据自己需要使用 每个人都可以上传相应版本配置到此仓库。格式：`版本.mv`(可以使用cmd查看

![image](https://user-images.githubusercontent.com/16742566/68569294-b9627900-0498-11ea-90c1-35d2f3af2ad6.png)

2. 一些UI逻辑调整
3. 其它版本也可以尝试使用（win7和win7sp1变化相差不大应该可以用，至于win10看天意...


#### 2019-11-10
0. 修复隐藏bug
1. 添加`MVConfigBuild.exe`生成私人配置文件，增强兼容性：`对相应已支持的系统即使在打了内核补丁的情况下可能也支持`。
- 之前支持：
> Microsoft Windows [版本 10.0.18362.**418**] //`19h1`
- 现在支持
>  Microsoft Windows [版本 10.0.18362.**xxx**] //`19h1`



2. 使用前自动检查系统版本、降低蓝屏几率




#### 2019-11-08
公开下载
