
五种 DevSecOps 提升安全性
======

![](https://opensource.com/sites/default/files/styles/image-full-size/public/lead-images/security-lock-password.jpg?itok=KJMdkKum)

对于我们是否需要扩展 DevOps 以确实提升安全性，我们一直都有争议。毕竟，我们的想法是，DevOps 一直是一系列的新实践的简写，使用新工具（通常是开源的）并且在这之上构建更多的协作文化。为什么 DevBizOps 不能更好地满足商业的需求？或者说 DevChatOps 强调的是更快更好的沟通？

在今年（译者注：此处是2018年）的早些时候写的关于他理解的 DevSecOps 术语，“我希望，有一天在世界范围内，我们能不再使用 DevSecOps 这个词，安全会是所有的服务交付讨论中理所应当的部分。直到那一天到来为止，在这一点上，我的一般性结论是，这个词只有三个新的特性。更重要的是，我们作为一个产业，在信息安全方面并没有做的很好，而这个名称切实地区分出了问题的状况”

所以，为什么我们在信息安全方面做的不好，在 DevSecOps 的语境下安全做的好又是什么意思呢？

我们大概从未做好过信息安全，尽管（也可能是因为）复杂的工业点产品地址拥挤问题。我们仍然可以在这个时代把工作做得足够好，以此来防范威胁，这些威胁主要集中在一个范围内，网络的连接是有限的，而且大多数的用户都是公司的员工，使用的是公司提供的设备。

这些年来，这些情况并没有能准确地描述出大多数组织的真实现状。但在现在这个时代，不止引入了 DevSecOps，也同时引入了新的应用架构模型，开发实践，和越来越多的安全威胁，这些一起定义了一个需要更快迭代的新常态。还没有应用得很多的 DevSecOps 在独立改变安全，但是 2018 年的信息安全需要新的方法。

请仔细思考下面这五个领域。

### 自动化

大量的自动化通常是 DevOps 的标志，这部分是关于速度的，如果你要快速移动（并且不会打坏东西），你需要有可重复的过程，而且这个过程不需要太多的人工干预。实际上，自动化是 DevOps 最好的切入点之一，甚至是在仍然主要工作在单片机电路程序的组织里也是如此。使用像 Ansible 这样易于使用的工具来自动化地处理相关的配置或者是测试，这是快速开始 DevOps 之路的常用方法。

DevSecOps 也不例外，在今天，安全已经变成了一个持续性的过程，而不是在应用的生命周期里进行不定期的检查，甚至是每周、每月的检查。当漏洞被厂商发现并修复的时候，这些漏洞能被快速地应用是很重要的，因为利用这些漏洞的利用程序很快就会被淘汰。

### "左转"

在开发流程结束时，传统安全通常被视作一个守门人。检查所有的部分确保没有问题，然后这个应用程序就可以投入生产了。否则，就要再来一次。所以安全团队的声誉并不高。

因此，我们想的是，没什么不把安全这个部分提到前面呢（左边是一个典型的从左到右的开发流程图）？安全性可能仍然不行，但在开发的早期进行重构的影响要远远小于开发已经完成并且准备上线时进行重构的影响。

不过，我不喜欢“左移”这个词，这意味着安全仍然是一个只不过提前进行的一次性工作。在应用程序的整个生命周期里，从供应链到开发，再到测试，直到上线部署，安全都需要进行大量的自动化处理。

### 管理依赖

我们在现代应用程序开发过程中看到的一个最大的改变，就是你通常不需要去编写这个程序的大部分代码。使用开源的函数库和框架就是一个明显的例子。但是你也可以从公共的云服务商或其他来源那里获得额外的服务。在许多情况下，这些额外的代码和服务比你给自己写的要好得多。

因此，DevSecOps 需要你把重点放在你的软件供应链上，你是从可信的来源那里获取你的软件的吗？这些软件是最新的吗？它们已经集成到了你为自己的代码使用的安全流程中了吗？对于这些你能使用的代码和 API 你有哪些策略？你为自己的产品代码使用的组件是否有可用的商业支持？

没有一套标准答案可以应对所有的情况。对于概念验证和大规模的生产，它们可能会有所不同。但是，正如制造业长期存在的情况（DevSecOps 和制造业的发展方面有许多相似之处），供应链的可信是至关重要的。

### 可见性

关于贯穿应用程序整个生命周期里所有阶段的自动化的需求，我已经谈过很多了。这里假设我们能看见每个阶段里发生的情况。

有效的 DevSecOps 需要有效的检测，以便于自动化程序知道要做什么。这个检测分了很多类别。一些长期的和高级别的指标能帮助我们了解整个 DevSecOps 流程是否工作良好。严重威胁级别的警报需要立刻有人进行处理（安全扫描系统已经关闭！）。有一些警报，比如扫描失败，需要进行修复。我们记录了大量的参数来生成日志，以便事后进行分析（随着时间的推移，哪些发生了改变？导致失败的原因是什么？）。

### 分散服务 vs 一体化解决方案

虽然 DevSecOps 实践可以应用于多种类型的应用架构，但它们对小型且松散耦合的组件最有效，这些组件可以进行更新和复用，而且不会在应用程序的其他地方进行强制更改。在纯净版的形式里，这些组件可以是微服务或者函数，但是这个一般性原则适用于通过网络进行通信的松散耦合服务的任何地方。

这种方法确实带来了一些新的安全挑战，组件之间的交互可能会很复杂，总的攻击面会更大，因为现在应用程序通过网络有了更多的切入点。

另一方面，这种类型的架构还意味着自动化的安全和监视可以更加精细地查看应用程序的组件，因为它们不再深埋在一整个应用程序之中。

不要过多地关注 DevSecOps 这个术语，但要提醒一下，安全正在不断地演变，因为我们编写和部署程序的方式也在不断地演变。

--------------------------------------------------------------------------------

via: https://opensource.com/article/18/9/devsecops-changes-security

作者：[Gordon Haff][a]
选题：[lujun9972](https://github.com/lujun9972)
译者：[hopefully2333](https://github.com/hopefully2333)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://opensource.com/users/ghaff
[1]: https://opensource.com/resources/devops
[2]: https://opensource.com/tags/devops
[3]: https://opensource.com/article/18/5/steps-apply-devops-culture-beyond-it
[4]: https://www.devsecopsdays.com/articles/its-just-a-name
[5]: https://opensource.com/article/18/4/devsecops
[6]: https://opensource.com/article/18/6/where-cycle-security-devops
[7]: https://opensource.com/tags/ansible
[8]: https://opensource.com/article/17/1/be-open-source-supply-chain
[9]: https://opensource.com/tags/microservices