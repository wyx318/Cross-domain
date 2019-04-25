# Cross-domain跨域与同源策略
浏览器出于安全方面的考虑，只允许与本域下的接口交互。不同源的客户端脚本在没有明确授权的情况下，不能读写对方的资源。

本域指的是？

- 同协议：如都是http或者https
- 同域名：如都是http://jirengu.com/a 和http://jirengu.com/b
- 同端口：如都是80端口
如：

http://jirengu.com/a/b.js 和 http://jirengu.com/index.php (同源)
不同源的例子：

- http://jirengu.com/main.js 和 https://jirengu.com/a.php (协议不同)
- http://jirengu.com/main.js 和 http://bbs.jirengu.com/a.php (域名不同，域名必须完全相同才可以)
- http://jiengu.com/main.js 和 http://jirengu.com:8080/a.php (端口不同,第一个是80)
需要注意的是: 对于当前页面来说页面存放的 JS 文件的域不重要，重要的是加载该 JS 页面所在什么域
