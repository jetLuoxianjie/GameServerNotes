sync.Cond的核心实现 - 通过一个锁，封装了notify 通知的实现，包括了单个通知与广播这两种方式
sync.Cond与channel的异同 - channel应用于一收一发的场景，sync.Cond应用于多收一发的场景