## macOS

mac 如何设置显示器 5 分钟后关闭，但是机器不休眠

```
sudo pmset displaysleep 5
sudo pmset -a sleep 0
```

## 禁止系统进入休眠的命令行工具 Caffeinate
Caffeinate 的使用非常简单，打开命令行，输入命令，保留命令行窗口（不要关闭）即可。如果中途不需要了，可以使用 control + z 来中断执行，或者直接关闭命令行窗口即可。

-s：禁止系统进入睡眠状态，此参数仅在插上电源的时候才有效。
-t：指定命令有效的超时值，以秒为单位。

caffeinate -s -t 9150446400
