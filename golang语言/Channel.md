channel用于Goroutine间通信时的注意点 - 合理设置channel的size大小 / 正确地关闭channel
合理地运用channel的发送与接收 - 运用函数传入参数的定义，限制 <- chan 和 chan <-
channel的底层实现 - 环形队列+发送、接收的waiter通知，结合Goroutine的调度思考
理解并运用channel的阻塞逻辑 - 理解channel的每一对 收与发 之间的逻辑，巧妙地使用
思考channel嵌套后的实现逻辑 - 理解用 chan chan 是怎么实现 两层通知 的？