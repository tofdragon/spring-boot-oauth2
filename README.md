# spring-boot-oauth2
spring boot, oauth2, spring security

环境要求：
jdk8
spring boot 2.0.1

运行:

启动成功后，用postman访问 GET请求 order/2 提示无权限 访问product/3 可以正常访问

使用postman获取access_token

POST请求:

http://localhost:8080/oauth/token?grant_type=password&username=bob&password=abc123

Authorization选项卡

Type: Basic Auth

Username: my-trusted-client

Password: secret

请求成功会响应access_token

GET请求:

http://localhost:8080/order/2?access_token=a375bb21-f090-4280-ac6a-98323da16e78 即可正常访问

