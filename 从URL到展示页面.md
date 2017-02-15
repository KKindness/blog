（本文内容为作者个人理解，有出现错误的地方欢迎指出）

第一步：在浏览器输入URL

URL：统一资源定位符，定位互联网上面的资源。

主要几个协议：

http协议：用于定位互联网资源，缺点是明文传输，不加密。
https协议：用于定位互联网资源并自带加密。（苹果公司强制iOS APP使用此协议，不出意外未来会取代http）
file协议：用于定位本地电脑资源
ftp协议：用于下载互联网资源（目前基本已被P2P取代，现多用于内网下载）

输入域名之后浏览器通过域名解析到IP，从而找到对应的服务器与之交互。
（为什么使用域名而不是直接使用IP？答：更容易记忆，方便宣传、传播。）

//开头等于和当前页面的协议保持一致。

第二步：域名解析

把域名解析成IP。

1.此浏览器缓存
2.本机hosts
3.你的路由器的缓存
4.ISP（服务商）的缓存
以上4个都没有就会去根服务器查找。

第三步：服务器处理

请求发给服务器，服务器端安装了Web server，用于接受请求、处理请求。

常见的Web server服务器软件有Apache、Nginx。

Web server作为入口，与用户产生交互，收到用户的请求之后发给网站代码或者其他的服务器。可以看作用户和服务器之间的桥梁。

![jirengu.png](http://upload-images.jianshu.io/upload_images/2597093-4bf1bda514efe6e8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

第四步：网站处理流程

MVC=模型（model）+视图（view）+控制器（controller）

M层与数据库进行交互，为C层提供数据。V层提供模版，把M层从数据库获取的数据添加到V层里面生成HTML传给C层。前端工程师主要负责V层。

HTML字符串传给浏览器，浏览器进行解析。浏览器在解析的过程会读取一些特殊的标签（比如图片img、脚本script）然后去服务器提取内容。最终浏览器根据HTML+CSS+javascript生成用户所看到的页面。


![jirengu2.png](http://upload-images.jianshu.io/upload_images/2597093-d731d17ffd66fa6a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)