# 应用名启动: 
- launchApp("appName")
- app.launchApp("appName")
***
# 包名启动:
- launch("com.app.package")
- app.launch("packageName)
***
# packageName与appName转换
- app.getPackageName("QQ") / getPackageName("QQ")
- app.getAppName("com.package.name") /getAppName("com.pakcage.name")
***
# 卸载应用
- app.uninstall("packageName")
***
# 浏览器打开某网址
- app.openUrl("url")
***
# 打开Autojs特定界面
- app.startActivity("console")
- app.startActivity("settings")