# 使用JHSDB分析Java对象
## 工具启动
在Java9之前没有JHSDB，需要使用JDK/lib/sa-jdi.jar来启动，启动命令

```
  (注意路径)
  java -cp .\sa-jdi.jar sun.jvm.hotspot.HSDB
  java -cp .\sa-jdi.jar sun.jvm.hotspot.CLHSDB
```
## 使用
1. 命令查找需要的进程
  `jps -l`  
  > 9584 com.hky.TestEgressPlaceTop  
  > 14804 org.jetbrains.jps.cmdline.Launcher  
  > 16964 sun.tools.jps.Jps  
  > 15848 org.jetbrains.idea.maven.server.RemoteMavenServer  
  > 6888  
  > 7320 sun.jvm.hotspot.HSDB  
2. 调用HSDB工具
  file>Attach to
