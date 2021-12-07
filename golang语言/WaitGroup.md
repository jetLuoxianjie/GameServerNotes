理解WaitGroup的实现 - 核心是CAS的使用
Add与Done应该放在哪？ - Add放在Goroutine外，Done放在Goroutine中，逻辑复杂时建议用defer保证调用
WaitGroup适合什么样的场景？ - 并发的Goroutine执行的逻辑相同时，否则代码并不简洁，可以采用其它方式