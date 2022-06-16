## 简介
Hyper Text Transfer Protocal over Secure Socket Layer

http的安全版，在http和tcp层之间加入了SSL/TLS层，用来实现内容加密、身份认证并保证数据完整性。

SSL(Secure Socket Layer)是加密套接字协议层，TLS(Transport Layer Security)是传输层安全协议，是SSL升级版

结构如下：
- 应用层(HTTP)
- 安全层(SSL/TLS)
- 传输层(TCP)
- 网络层(IP)
- 链路层

http和https主要区别：
- http是明文传输，https是加密传输
- http使用80端口，https使用443端口
- https使用时要对数据加密和解密，效率相对http低
- https需要CA机构的证书

## 认证类型



