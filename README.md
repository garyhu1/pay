# pay
银联支付

##银联下载地址
[zip](https://open.unionpay.com/ajweb/help/file/techFile?productId=3)

### 远程端连接信息配置
```java
    socketClient.getAddress().setRemoteIP(IPUtil.getLocalIPAddress(true)); // 远程端IP地址
    socketClient.getAddress().setRemotePort("21998"); // 远程端端口号
    socketClient.getAddress().setConnectionTimeout(15 * 1000); // 连接超时时长，单位毫秒
```
