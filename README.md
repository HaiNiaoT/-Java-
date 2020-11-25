<h1>使用JHSDB分析Java对象</h1>
<h2>工具启动</h2>
在Java9之前没有JHSDB，需要使用JDK/lib/sa-jdi.jar来启动，启动命令
`
  (注意路径)
  java -cp .\sa-jdi.jar sun.jvm.hotspot.HSDB
  java -cp .\sa-jdi.jar sun.jvm.hotspot.CLHSDB
`
  
