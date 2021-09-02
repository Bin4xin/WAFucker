# WAFucker

互联网发展至今将近三十余年，当下随着信息网络的不断发展全球信息化进程不断加速，网络安全行业从而也迎来新机遇、新挑战；

- 现为：
	- 进一步规范各项目间相关工作流程；
	- 进一步优化各项目产能，弥补技能短板；
	- 沉淀相关安全技术和培养相关技术人才；

开源出相关技术WIKI；此仓库为WAF相关，故起名[WAFucker](https://github.com/Bin4xin/WAFucker) - Power By Bin4xin :D

## ***请注意!!!ATTENTION PLZ!!!***

您若下载并使用该仓库应充分认知并理解：
    
- 1.没有预先经过同意，被看作未授权攻击的：包括但不限于有意避开系统访问控制机制，对网络设备及资源进行非正常使用，或擅自扩大权限，越权访问信息；
- 2.由于第三方（人、平台）传播、二次开发、脚本滥用等行为而造成的任何直接或者间接的后果及损失跟作者无关，均由使用者本人负责，本文作者不为此承担任何责任，仅做技术讨论和分享；
- 3.尊重他人劳动成果，使用请申明出处：[WAFucker](https://github.com/Bin4xin/WAFucker)。

If you download and use the repository, you should fully recognize and understand:

- i. Unauthorized attacks without prior consent: including but not limited to deliberately evading system access control mechanisms, making abnormal use of network equipment and resources, or expanding permissions without authorization, and accessing information without authorization;
- ii. Any direct or indirect consequences and losses caused by third-party (person, platform) dissemination, secondary development, script abuse, etc. have nothing to do with the author and are the responsibility of the user himself, and the author of this article does not bear any responsibility for this responsibility. Only for technical discussion and sharing;
- iii. Respect personal labor results, prohibit commercial use. Personal use please state the source: [WAFucker](https://github.com/Bin4xin/WAFucker).

## 零：是什么？

### # 0x01：什么是WAF？

*Web应用防护墙或又叫网页应用及入侵防御系统(英文：Web Application Firewall)*是通过执行一系列针对*HTTP/HTTPS*的安全策略来专门为*Web*应用提供保护的一款产品；

主要用于防御针对网络应用层的攻击，如*SQL注入、跨站脚本攻击、参数篡改、应用平台漏洞攻击、拒绝服务攻击等*

### # 0x02：[怎么识别WAF？](https://github.com/Bin4xin/WAFucker/tree/master/WAF%E8%AF%86%E5%88%AB)

## 一：为什么做？

我们在实际的渗透测试过程中，经常会碰到网站存在WAF的情况。网站存在WAF，意味着我们不能使用安全工具对网站进行测试，因为一旦触碰了WAF的规则，轻则丢弃报文，重则拉黑IP。

所以，我们需要手动进行WAF的绕过，这样也是我们的最终目标，能够尽可能绕过WAF来进行渗透测试，防止其作“拦路虎”。


## 二：怎么做？

绕过WAF前肯定需要对WAF的工作原理有一定的理解。本文主要从绕过WAF过程中的注意点出发，尝试理解WAF的运作，构建一个简单的知识框架。

### # 2x01：[怎么绕过WAF](https://github.com/Bin4xin/WAFucker/tree/master/WAF%E7%BB%95%E8%BF%87)

## 三：其他拓展

### # 3x01：[怎么开发WAF](https://github.com/Bin4xin/WAFucker/tree/master/WAF%E5%BC%80%E5%8F%91)

## 四：参考

- [WAF的工作原理和绕过浅析](https://blog.csdn.net/qq_36119192/article/details/90113167)
- [什么是WAF](https://www.huaweicloud.com/zhishi/dyl46.html)