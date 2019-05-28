### 代码注入、命令执行

	1.内置危险函数
	exec
	execfile
	eval
	
	2.标准库危险模块
	os
	subprocess
	commands
	
	3.危险第三方库
	Template(user_input) : 模板注入(SSTI)所产生的代码执行
	subprocess32 
	
	4.反序列化
	marshal
	PyYAML
	pickle和cpickle
	shelve
	PIL
	unzip


[Python沙箱逃逸的n种姿势](https://xz.aliyun.com/t/52)

[禁用import的情况下绕过python沙箱](https://www.anquanke.com/post/id/107000)

[Escaping the Python Sandbox](https://zolmeister.com/2013/05/escaping-python-sandbox.html)

[Python Sandbox Bypass](https://mp.weixin.qq.com/s?__biz=MzIzOTQ5NjUzOQ==&mid=2247483665&idx=1&sn=4b18de09738fdc5291634db1ca2dd55a)

[Python之数据序列化（json、pickle、shelve）](http://www.cnblogs.com/yyds/p/6563608.html)

[Exploiting Python PIL Module Command Execution Vulnerability](https://xz.aliyun.com/t/44)

[Exploiting Python Code Injection in Web Applications](https://www.doyler.net/security-not-included/exploiting-python-code-injection)

[EXPLOITING PYTHON CODE INJECTION IN WEB APPLICATIONS](http://www.securitynewspaper.com/2016/11/12/exploiting-python-code-injection-web-applications/)

[Python eval的常见错误封装及利用原理](http://xxlegend.com/2015/07/31/Python%20eval%E7%9A%84%E5%B8%B8%E8%A7%81%E9%94%99%E8%AF%AF%E5%B0%81%E8%A3%85%E5%8F%8A%E5%88%A9%E7%94%A8%E5%8E%9F%E7%90%86/)

[Exploiting Python’s Eval](http://www.floyd.ch/?p=584)

[Exploiting insecure file extraction in Python for code execution](https://ajinabraham.com/blog/exploiting-insecure-file-extraction-in-python-for-code-execution)

[掌阅iReader某站Python漏洞挖掘](https://www.leavesongs.com/PENETRATION/zhangyue-python-web-code-execute.html)

[Python Pickle的任意代码执行漏洞实践和Payload构造](http://code2sec.com/python-picklede-ren-yi-dai-ma-zhi-xing-lou-dong-shi-jian-he-payloadgou-zao.html)

[django的secret key泄漏导致的命令执行实践](http://code2sec.com/djangode-secret-keyxie-lou-dao-zhi-de-ming-ling-zhi-xing-shi-jian.html)

[Remote Code Execution on a Facebook server](https://blog.scrt.ch/2018/08/24/remote-code-execution-on-a-facebook-server/)

[Python PyYAML反序列化漏洞实验和payload构造](http://www.code2sec.com/2017/09/22/python-pyyaml%E5%8F%8D%E5%BA%8F%E5%88%97%E5%8C%96%E6%BC%8F%E6%B4%9E%E5%AE%9E%E9%AA%8C%E5%92%8Cpayload%E6%9E%84%E9%80%A0/)

[Exploiting Python Deserialization Vulnerabilities](https://crowdshield.com/blog.php?name=exploiting-python-deserialization-vulnerabilities)

[Shellcoding in Python’s serialisation format](https://media.blackhat.com/bh-us-11/Slaviero/BH_US_11_Slaviero_Sour_Pickles_WP.pdf)

[PyCodeInjection代码注入实验环境](https://github.com/sethsec/PyCodeInjection)

[Exploiting Python Code Injection in Web Applications](https://sethsec.blogspot.com/2016/11/exploiting-python-code-injection-in-web.html)  （[翻译版](https://www.anquanke.com/post/id/84891)）

[Numpy反序列化命令执行(CVE-2019-6446)浅析](https://www.freebuf.com/vuls/194540.html)



### 代码审计

[Python安全编码和代码审计](http://xxlegend.com/2015/07/30/Python%E5%AE%89%E5%85%A8%E7%BC%96%E7%A0%81%E5%92%8C%E4%BB%A3%E7%A0%81%E5%AE%A1%E8%AE%A1/)

[Python代码审计连载之一：CSRF](https://xz.aliyun.com/t/391) 同  <https://www.cdxy.me/?p=736> 

[Python代码审计连载之二：SSTI](https://xz.aliyun.com/t/390)  同 <https://www.cdxy.me/?p=738> 

[Python代码审计连载之三：Server Side Request](https://xz.aliyun.com/t/389) 同  <https://www.cdxy.me/?p=744> 

[Python代码审计连载之四：Command Execution](https://xz.aliyun.com/t/388) 同  <https://www.cdxy.me/?p=747> 

[Dangerous Python Functions, Part 1](https://www.kevinlondon.com/2015/07/26/dangerous-python-functions.html)

[Dangerous Python Functions, Part 2](https://www.kevinlondon.com/2015/08/15/dangerous-python-functions-pt2.html)

[Dangerous Python Functions, Part 3](https://www.kevinlondon.com/2017/01/30/dangerous-python-functions-pt3.html)

[记一下PythonWeb代码审计应该注意的地方](http://blog.neargle.com/2016/07/25/log-of-simple-code-review-about-python-base-webapp/)

[廖新喜大佬的python代码审计工具](https://github.com/shengqi158/pyvulhunter)

[来自openstack安全团队的python代码静态审计工具](https://github.com/openstack/bandit)

[来自openstack安全团队的python代码静态审计工具2](https://github.com/openstack/syntribos)

[代码审计工具pyt](https://github.com/python-security/pyt)

[xfkxfk的python自动化代码审计](https://mp.weixin.qq.com/s?__biz=MzUxOTYzMzU0NQ==&mid=2247483887&idx=1&sn=99ab12309de75381e37c058d53def1b6&chksm=f9f7ee09ce80671fc5887a9c25350fc610559cc1e095f9b689473873889581e4c5fbb0dec2cd&mpshare=1&) 基于[pyekaboo](https://github.com/SafeBreach-Labs/pyekaboo) 和廖新喜的[pyvulhunter](https://github.com/shengqi158/pyvulhunter)



### Django相关

[Django debug page XSS漏洞（CVE-2017-12794）分析](https://www.leavesongs.com/PENETRATION/django-debug-page-xss.html)

[Django DeleteView without confirmation template, but with CSRF attack](https://www.leavesongs.com/PYTHON/django-deleteView-without-confirmation-template.html)

[Django安全机制](http://xxlegend.com/2015/04/01/Django%E5%AE%89%E5%85%A8%E6%9C%BA%E5%88%B6/)

[从Django的SECTET_KEY到代码执行](http://xxlegend.com/2015/04/01/%E4%BB%8EDjango%E7%9A%84SECTET_KEY%E5%88%B0%E4%BB%A3%E7%A0%81%E6%89%A7%E8%A1%8C/)

[Django CSRF Bypass (CVE-2016-7401) 漏洞分析](https://paper.seebug.org/58/)

[Django CSRF Bypass 漏洞分析(CVE-2016-7401)](http://blog.knownsec.com/2016/10/django-csrf-bypass_cve-2016-7401/)

[Django的两个url跳转漏洞分析:CVE-2017-7233&7234](https://paper.seebug.org/274/)

[Python 格式化字符串漏洞（Django为例）](https://www.leavesongs.com/PENETRATION/python-string-format-vulnerability.html) 同 https://xz.aliyun.com/t/288

[Django 安全最佳实践](http://www.atjiang.com/2scoopsdjango1.8-26-security-best-practices/)

[从Pwnhub诞生聊Django安全编码](https://www.leavesongs.com/PYTHON/django-coding-experience-from-pwnhub.html)

[python和django的目录遍历漏洞(任意文件读取)](http://www.lijiejie.com/python-django-directory-traversal/)

[新型任意文件读取漏洞的研究](https://www.leavesongs.com/PENETRATION/arbitrary-files-read-via-static-requests.html)

[django的一些安全问题答案](https://www.kevinlondon.com/2015/10/16/answers-to-django-security-questions.html)



### package钓鱼

[Package 钓鱼](https://paper.seebug.org/311/)

[被忽视的攻击面：Python package 钓鱼](https://paper.seebug.org/326/)

https://www.pytosquatting.org/



### LDAP注入

[Python安全编码之预防LDAP注入](http://xxlegend.com/2016/12/01/Python%E5%AE%89%E5%85%A8%E7%BC%96%E7%A0%81%E4%B9%8B%E9%A2%84%E9%98%B2LDAP%E6%B3%A8%E5%85%A5/)



### SSRF

[谈一谈如何在Python开发中拒绝SSRF漏洞](https://www.leavesongs.com/PYTHON/defend-ssrf-vulnerable-in-python.html)

[Python安全 - 从SSRF到命令执行惨案](https://www.leavesongs.com/PENETRATION/getshell-via-ssrf-and-redis.html)

[Splash SSRF 到获取内网服务器 ROOT 权限](https://xz.aliyun.com/t/118)



### XSS

[Flask Debugger页面上的通用XSS漏洞分析和挖掘过程记录](http://blog.neargle.com/2016/09/21/flask-src-review-get-a-xss-from-debuger/)



### SQLI

[讨论PythonWeb开发中可能会遇到的安全问题之SQL注入](http://blog.neargle.com/2016/07/22/pythonweb-framework-dev-vulnerable/)



### SSTI模版注入

[Python Security Auditing (II): SSTI](https://www.cdxy.me/?p=738)

[exploring-ssti-in-flask-jinja2](https://nvisium.com/blog/2016/03/09/exploring-ssti-in-flask-jinja2/)

[exploring-ssti-in-flask-jinja2-part-ii](https://nvisium.com/blog/2016/03/11/exploring-ssti-in-flask-jinja2-part-ii/)



### python webshell

https://github.com/evilcos/python-webshell

https://github.com/ahhh/Reverse_DNS_Shell

### paper

Python_Hack_知道创宇_北北(孙博).pdf

### 其他

[如何判断目标站点是否为Django开发](https://www.leavesongs.com/PENETRATION/detect-django.html)

[Supervisord远程命令执行漏洞（CVE-2017-11610）](https://www.leavesongs.com/PENETRATION/supervisord-RCE-CVE-2017-11610.html)

[python富文本XSS过滤器](https://www.leavesongs.com/PYTHON/python-xss-filter.html)

[基于mezzanine的攻防比赛环境搭建及XXE漏洞构造/](http://xxlegend.com/2016/04/01/%E5%9F%BA%E4%BA%8Emezzanine%E7%9A%84%E6%94%BB%E9%98%B2%E6%AF%94%E8%B5%9B%E7%8E%AF%E5%A2%83%E6%90%AD%E5%BB%BA%E5%8F%8AXXE%E6%BC%8F%E6%B4%9E%E6%9E%84%E9%80%A0/)

[Python Waf黑名单过滤下的一些Bypass思路](http://www.0aa.me/index.php/archives/123/)

[Pwnhub Web题Classroom题解与分析](https://www.leavesongs.com/PENETRATION/pwnhub-web-classroom-django-sql-injection.html)

[Programming Secure Web Applications in Python](https://www.thoughtco.com/programming-secure-web-applications-2813531)

[[CVE-2016-5699] HTTP Header Injection in Python urllib](http://blog.blindspotsecurity.com/2016/06/advisory-http-header-injection-in.html) 同 http://www.anquan.us/static/drops/papers-16905.html

[[CVE-2019-9740] Python urllib CRLF injection vulnerability](https://bugs.python.org/issue36276)  同 https://xz.aliyun.com/t/5123

[Hack Redis via Python urllib HTTP Header Injection](https://security.tencent.com/index.php/blog/msg/106)

[【技术分享】python web 安全总结](http://bobao.360.cn/learning/detail/4522.html)



### 安全工具

[python正向连接后门](https://www.leavesongs.com/PYTHON/python-shell-backdoor.html)

[struts2 S2-016/S2-017 Python GetShell](https://www.leavesongs.com/PENETRATION/UseOfStruts.html)

[Python多线程端口扫描工具](https://www.leavesongs.com/PYTHON/PortScanner.html)

[Python JSON Fuzzer: PyJFuzz](https://n0where.net/python-json-fuzzer-pyjfuzz/)

https://github.com/smartFlash/pySecurity



### 对象注入、底层安全

[DEFENCELY CLARIFIES PYTHON OBJECT INJECTION EXPLOITATION](https://defencely.com/blog/defencely-clarifies-python-object-injection-exploitation/)

[OWASP Python Security Project](https://github.com/ebranca/owasp-pysec)

[Escaping a Python sandbox with a memory corruption bug](https://hackernoon.com/python-sandbox-escape-via-a-memory-corruption-bug-19dde4d5fea5)