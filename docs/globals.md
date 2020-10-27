# 全局函数
- sleep(1000);  // 睡眠1秒
- currentPackage()  // return string 当前运行包名 依赖无障碍
- currentActivity() // return string 当前Activity名 依赖无障碍
## 剪切板
- setClip("text") // 设置剪切板文字
- getClip() // 获取当前剪切板内容
## 气泡消息提醒
- toast("message")
- 默认显示2秒(具体时间取决于安卓系统，可手动封装自己的toast)
````Javascript
var old_toast = toast;
toast = function(message, duration) {
  old_toast(message)
  sleep(3000) // sleep函数会阻塞其他操作吗？
}
````
- toastLog("message"): 相当于toast(message); log(message);
## 等待指定应用/页面
- waitForActivity(activity[,period=200]): activity名称，轮询等待时间：等待指定Activity出现
- waitForPackage(package[,period=200]): 等待指定应用出现
## 停止脚本运行
- exit(): 立即停止脚本运行，是通过异常实现的 因此别用try...catch
## 随机数
- random(): return 随机浮点数在0到1之间
- random(min, max): 随机返回给定范围内的数
## 脚本运行条件检测
- requiresApi(apiNumber)
- requiresAutojsVersion(versionString|versionNumber)
## 动态申请手机权限
- runtime.requestPermissions(["access_fine_location","record_audio"])