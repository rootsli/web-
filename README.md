1.	JS代码检测工具：http://www.jslint.com/
2.	代码调试工具：firedebug，IE自带的开发人员调试工具，google Chromium自带的开发人员调试工具
3.	性能评估工具：Yslow插件，http://developer.yahoo.com/yslow/
4.	代码压缩工具：http://dean.edwards.name/packer/
5.	图片压缩工具：http://www.smushit.com/ysmush.it/
6.	使用Data URIS技术：该技术可以将css中的图片编码成2进制后嵌入css文件中，以减少http请求数
7.	浏览器兼容性测试：http://browsershots.org/
8.	图片资源搜索：http://findicons.com/
9.	本地代码版本管理：VisualSVN-Server-2.1.7.msi
10.	浏览器兼容性检测：Modernizr (modernizr.com) 提供了一种更好的方法。 Modernizr 是一个 JavaScript 库，用于“…检测是否可以使用下一代 Web 技术（也就是来源于 HTML5 和 CSS3 规范的功能）的本地实现 
http://msdn.microsoft.com/zh-cn/magazine/hh394148.aspx、
11.	代码文件最好使用utf-8 不带签名的编码格式保存，以防止出现乱码
12.	使用jsdoc自动生成API文档
13.	遵循Google JavaScript 编码规范指南.doc，Google HTML,CSS编码规范指南.doc
14.	关于http post两阶段提交的一些问题:使用AJAX的post方法进行数据提交的时候，数据段分2次传输，如果2次传输间时间间隔过大，会引起服务器超时，而引起访问错误。http://blog.csdn.net/axman/article/details/7663002
15.	js在线格式化：http://jsbeautifier.org/
16.	代码在线调试：http://jsfiddle.net/

一些web资源：
1.	强大的免费图标搜索引擎：http://browsershots.org/
2.	几个基于jquery的画图插件：
http://www.jqplot.com/
https://github.com/flot/flot.github.com
http://www.highcharts.com/
http://omnipotent.net/jquery.sparkline/#s-about（mini chart）

yahoo建议优化标准：
(1)	使用尽可能少的http请求（Make fewer HTTP requests）
(2)	使用CDN（Use a CDN）
(3)	避免空的src和href（Avoid empty src or hre）
(4)	Html增加Expires头（Add Expires headers）--html中设置Expires只对html有效，对js，css及图片无效，最好在服务器端设置该参数
(5)	使用GZIP压缩组件（Compress components with GZip）
(6)	把CSS放在html顶部（Put CSS at top）
(7)	把javascript放在html底部（Put JavaScript at bottom）
(8)	避免使用css表达式（Avoid CSS expressions）
(9)	单独放置js和css文件(Make JavaScript and CSS external)
(10)	减少DNS查询（Reduce DNS lookups）
(11)	压缩js和css（Minify JavaScript and CSS）
(12)	避免URL重定向（Avoid URL redirects）
(13)	移除相同的js和css（Remove duplicate JavaScript and CSS）
(14)	配置ETags（Configure ETags）
(15)	缓存AJAX（Make AJAX cacheable）
(16)	AJAX使用get方式请求（Use GET for AJAX requests）
(17)	减少dom元素的数量（Reduce the number of DOM elements）
(18)	尽量避免404错误（Avoid HTTP 404 (Not Found) error）
(19)	减小Cookie大小（Reduce cookie size）
(20)	Use cookie-free domains
(21)	Avoid AlphaImageLoader filter
(22)	Do not scale images in HTML
(23)	Make favicon small and cacheable
17.	aa
18.	bb
19.	cc

其他的web优化建议：
https://developers.google.com/speed/docs/best-practices/rules_intro?hl=zh-CN
http://developer.yahoo.com/performance/rules.html

浏览器的工作原理：
http://taligarsiel.com/Projects/howbrowserswork1.htm
 
http://ux.sohu.com/topics/50972d9ae7de3e752e0081ff


XHTML规范：
1.文件类型声明：<!DOCTYPE（声明DTD类型） html（声明根元素） PUBLIC（声明公共标识符）
"-//W3C//DTD XHTML 1.0 Transitional//EN"（公共标识符）
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"（dtd类型）>
2.元素必须被正确地嵌套
3.使用小写的标签和属性名
4.给所有属性加上引号，为所有的属性分配值
5.属性不能简写，例：checked="checked"
6.用 id 属性代替 name 属性
7.关闭所有的标签，非空标签必须使用结束标签，使用空格和斜线关闭空标签，例：<hr /> 和 <br />。
8.不要在注释中写双下划线。
9.确保小于号及和号为 < 和 &
10.XML、XHTML、和HTML 4.0 文档的默认字符集是 Unicode，一个由 Unicode 联盟定义的标准
11.XHTML 文档必须拥有一个根元素，html

优秀的设计=界面美工（界面设计、图片设计）+交互模式+信息集成+用户使用习惯+创新型设计+响应速度
交互设计+美工设计


常见web攻击：
1.	CSRF/XSRF（Cross Site Request Forgery, 跨站域请求伪造）
2.	SQL 脚本注入
3.	跨站脚本攻击XSS
4.	重定向漏洞
5.	缓冲区溢出
(24)	反射型 XSS 漏洞
(25)	保存型 XSS 漏洞
(26)	重定向漏洞
(27)	本站点请求漏洞
(28)	跨站点请求漏洞
(29)	SQL 注入漏洞

以下内容来自：http://www.ibm.com/developerworks/cn/web/wa-secxss/
下面是站点管理员和开发人员可用来阻止 XSS 攻击的检查列表：
•	保证 Web 站点的页面只有在验证了用户输入没有恶意代码之后才返回用户输入。
•	在验证的同时过滤输入中的 Meta 字符。（这是消除 XSS 攻击的一个重要检查点。虽然它不能消除全部的 XSS 问题，但它能警告 Web 维护人员在站点安全性方面存在的不足）。
•	不要完全相信使用了 HTTPS（Secure Sockets Layer）的 Web 站点就不会受到 XSS 攻击；HTTPS 只能确保安全连接，处理用户输入的数据是应用程序内部的事情。如果应用程序有 XSS 漏洞，攻击者就可能会发送能被应用程序执行的恶意脚本，导致 XSS 侵入。
•	在搜索引擎和论坛内显示用户输入之前，将所有非字母和数字字符转变成 HTML 字符。
•	在应用程序正式付诸使用之前，在设计阶段大量使用测试工具，消除这类 XSS 漏洞。（强调这点的最佳实践指南具有 Extreme Programming 提到的思想）。
•	开发一些具有私有和公共密钥的标准或标志脚本，这些脚本要确实进行检查，以保证所引入的脚本真正经过了身份验证。（要大规模地实现，Internet 规则就必须进行标准化，以得出一套由 W3C 等主要参与者参与的公认方法）。


UI设计原则：
1.最少步骤，最高效率
2.进入一个页面，页面显示的内容是否是80%用户所需要的。剩下20%用户的需求要如何满足。
3.少即是多
4.符合用户习惯，预防错误
5. 一致性， 简洁性， 避免干扰和打断，减轻用户记忆负担，及时有效的反馈，让用户放松心态，不怕犯错
6.使用拖动，连线等设计方式
7.良好的文字提示：一致性，简洁性
8.如果可能，提供用户个性化定制
9.光标应该定位到恰当位置，适当时候，选中文本；“返回”时光标应该定位至何处等；
10.提供帮助文档
11.设计是一种平衡
12.应该提供向导功能
13.提供给用户反馈渠道

  
 

Web网管应该具备的基本功能：
1.      超时要求重新认证
2.      用户权限管理
3.      支持定义管理员IP范围，允许哪些IP访问Web，哪些不可以
4.      及时反馈配置结果，成功，info，warning，error及原因
5.      管理Web登陆用户
6.      页面快速的响应
7.      版权声明
8.      用户名密码加密传输

使用GruntJS构建Web开发环境：（介绍用GrunJS合并压缩js，css）:
http://www.cnblogs.com/snandy/archive/2013/03/07/2946989.html
http://www.cnblogs.com/snandy/archive/2013/03/11/2949177.html
http://www.cnblogs.com/snandy/archive/2013/05/20/3088613.html
http://www.zfanw.com/blog/gruntjs-optimize-image-size-loseless.html





















 
 


 
