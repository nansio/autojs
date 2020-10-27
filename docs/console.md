# 控制台
## 显示隐藏
- console.show()
- console.hide()
- console.clear()
## 输出
- console.log([data][,...args])
- console.verbose([data][,...args]) : 输出以灰色字体显示，优先级低于log
- console.info([data][,...args]): 绿色字体，优先级高于log, 重要信息
- console.warn([data][,...args]): 蓝色字体，优先级高于info,警告信息
- console.error([data][,...args]): 红色字体，由下级高于warn, 错误信息
- console.assert(test, message): 断言的bool值, 输出错误信息 停止脚本运行
- console.time([label]): 启动定时器, label作为定时器标识
- console.timeEnd(label): 停止指定标识的计时器
## 输入
- console.rawInput("message"): 字符串
- console.input("message"): 使用eval计算返回
## 大小
- console.setSize(width, height): number
````javascript
console.setSize(device.width/2, device.height/2);
````
## 位置
- console.setPosition(x, y): 横纵坐标
