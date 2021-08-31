# WAFucker - 识别

- 首先，WAF分为非嵌入型WAF和嵌入型WAF；
	- 非嵌入型WAF指的是硬件型WAF、云WAF、软件型WAF之类；
	- 嵌入型WAF指的是网站内置的WAF；

非嵌入型WAF对Web流量的解析完全是靠自身的，而嵌入型WAF拿到的Web数据是已经被解析加工好的。

所以非嵌入型的受攻击机面还涉及到其他层面，而嵌入型WAF从Web容器模块型WAF、代码层WAF往下走，其对抗畸形报文、扫操作绕过的能力越来越强。当然，在部署维护成本方面，也是越高的。









- 参考
	- [盘点：常见WAF进程/服务与WAF识别总结](https://www.secrss.com/articles/27147)
