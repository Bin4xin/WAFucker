# WAFucker

互联网发展至今将近三十余年，当下随着信息网络的不断发展全球信息化进程不断加速，网络安全行业从而也迎来新机遇、新挑战；

- 现进一步规范各项目间相关工作流程：
	- 进一步优化各项目产能，弥补技能短板；
	- 沉淀相关安全技术和培养相关技术人才；

开源出的相关技术WIKI

## ***请注意!!!ATTENTION PLZ!!!***

您若下载并使用该仓库应充分认知并理解：
    
- 1.没有预先经过同意，被看作未授权攻击的：包括但不限于有意避开系统访问控制机制，对网络设备及资源进行非正常使用，或擅自扩大权限，越权访问信息；
- 2.由于第三方（人、平台）传播、二次开发、脚本滥用等行为而造成的任何直接或者间接的后果及损失跟作者无关，均由使用者本人负责，本文作者不为此承担任何责任，仅做技术讨论和分享；
- 3.尊重他人劳动成果，使用请申明出处：[WAFucker](https://github.com/Bin4xin/WAFucker)。


If you download and use the repo, you should fully recognize and understand:

- i. Unauthorized attacks without prior consent: including but not limited to deliberately evading system access control mechanisms, making abnormal use of network equipment and resources, or expanding permissions without authorization, and accessing information without authorization;
- ii. Any direct or indirect consequences and losses caused by third-party (person, platform) dissemination, secondary development, script abuse, etc. have nothing to do with the author and are the responsibility of the user himself, and the author of this article does not bear any responsibility for this responsibility. Only for technical discussion and sharing;
- iii. Respect personal labor results, prohibit commercial use . Personal use please state the source: [WAFucker](https://github.com/Bin4xin/WAFucker).

## 零：是什么？

### # 0x01：什么是WAF？

**Web应用防护墙/网页应用及入侵防御系统（Web Application Firewall，简称WAF）**是通过执行一系列针对HTTP/HTTPS的安全策略来专门为Web应用提供保护的一款产品；

主要用于防御针对网络应用层的攻击，像*SQL注入、跨站脚本攻击、参数篡改、应用平台漏洞攻击、拒绝服务攻击等*


- 参考
 	- [什么是WAF](https://www.huaweicloud.com/zhishi/dyl46.html)

## 一：为什么做？

在实际的渗透测试过程中，经常会碰到网站存在WAF的情况。网站存在WAF，意味着我们不能使用安全工具对网站进行测试，因为一旦触碰了WAF的规则，轻则丢弃报文，重则拉黑IP。所以，我们需要手动进行WAF的绕过，而绕过WAF前肯定需要对WAF 的工作原理有一定的理解。本文主要从绕过WAF过程中需要注意的角色和点出发，尝试理解它们的运作，构建一个简单的知识框架。

首先，WAF分为非嵌入型WAF和嵌入型WAF，非嵌入型WAF指的是硬件型WAF、云WAF、软件型WAF之类的；而嵌入型WAF指的是网站内置的WAF。非嵌入型WAF对Web流量的解析完全是靠自身的，而嵌入型WAF拿到的Web数据是已经被解析加工好的。所以非嵌入型的受攻击机面还涉及到其他层面，而嵌入型WAF从Web容器模块型WAF、代码层WAF往下走，其对抗畸形报文、扫操作绕过的能力越来越强。当然，在部署维护成本方面，也是越高的。


- 参考
	- [WAF的工作原理和绕过浅析](https://blog.csdn.net/qq_36119192/article/details/90113167)



## 二：怎么做？