# cache
缓存库，支持caffeine、guava、redis、redis-cluster，支持两级缓存配置，支持布隆过滤器

## Maven依赖：
```xml
<dependency>
    <groupId>com.github.duanxinyuan</groupId>
    <artifactId>library-cache</artifactId>
    <version>1.2.0</version>
</dependency>
```

## 使用示例：
    Cache cache = Cache.getInstance();
    
    普通字符串操作：
    cache.set
    cache.get
    cache.del
    cache.exists
    cache.expire
    cache.persist
    
    //键值对原子操作
    cache.setnx
    
    //list操作
    cache.lpush
    cache.rpush
    cache.lindex
    cache.lrangePage
    cache.lrem
    
    //set操作
    cache.sadd
    cache.sismember
    cache.smembers
    
    //map操作
    cache.hset
    cache.hmset
    cache.hget
    cache.hgetAll
    
    //hyperloglog操作
    cache.pfadd
    cache.pfcount
  
    //bitmap操作
    cache.setbit
    cache.getbit
    cache.bitcount
    cache.bitop
    cache.bitfield
    cache.bitpos
  
    //bloomfilter
    cache.bloomadd
    cache.bloomcons
