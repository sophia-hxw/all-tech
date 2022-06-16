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

### 单向认证
目前大多数app和服务端的https连接都是单向；

只在app端对服务器进行验证，服务器不对app端进行验证；

在服务器端配置证书，app端不配置证书；

app发送请求时，将http换成https即ok

### 双向认证

除了单向验证的要求，另外，客户端也要配置证书

通常是企业级应用对接

双向验证科包含特定信息，所以不再需要用户手动输入用户名和密码，对不需要用户操作、自动运行的app尤其有用


