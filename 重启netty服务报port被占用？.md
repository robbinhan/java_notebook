# 重启Netty服务报port被占用？

添加以下设置

```java
Configuration config = new Configuration();
config.getSocketConfig().setReuseAddress(true);
```

 

