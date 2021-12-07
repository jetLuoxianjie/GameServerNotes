sync.Pool的核心作用 - 读源码，缓存稍后会频繁使用的对象+减轻GC压力
sync.Pool的Put与Get - Put的顺序为local private-> local shared，Get的顺序为 local private -> local shared -> remote shared
思考sync.Pool应用的核心场景 - 高频使用且生命周期短的对象，且初始化始终一致，如fmt
探索Go1.13引入victim的作用 - 了解victim cache的机制