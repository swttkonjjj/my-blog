reddit原文：[Automatic1111没有做错什么，有些人正试图摧毁它。](https://www.reddit.com/r/StableDiffusion/comments/y1uuvj/automatic1111_did_nothing_wrong_some_people_are/)

![image-20221017112504812](https://picgo-swtt.oss-cn-beijing.aliyuncs.com/image-20221017112504812.png)

在文章，作者试图解释NovelAi和automatic111webui之间争议的最相关事件。

词汇表（针对实际用途简化）：

- NovelAI: 人工智能图像生成的每月订阅服务。
- Automatic: Automatic1111 web Ui的创建者。
- Automatic1111: [u/AUTOMATIC1111](https://www.reddit.com/u/AUTOMATIC1111/) 用户创建的Stable Diffusion web UI 。是最流行的web ui之一。
- Emad: Stability AI公司创始人兼CEO(开发Stable Diffusion 的公司).
- RNN: 循环神经网络。（一种神经网络）。
- Weight(权重): 一些机器学习模型的参数。
- Model(模型): 基于可用数据模拟逻辑决策的机器学习算法。



**1st event:** (根据用户[u/AUTOMATIC1111](https://www.reddit.com/u/AUTOMATIC1111/))对事件的说法)NovelAI 从Automatic1111 web ui[克隆了同样的代码](https://i.imgur.com/jgyvup5.png) 并进行修改，以便在其业务中使用。

![jgyvup5](https://picgo-swtt.oss-cn-beijing.aliyuncs.com/jgyvup5.png)

>昨天我和一位开发人员进行了一次非常疲劳的讨论。我来要求他不要再说我偷了代码因为我没有，他一直在谈论道德谴责和伤害人。当他们这么说的时候你在道义上应受谴责就没有理由来。
>
>顺便说一句，我确实检查了代码，NAl正在使用我的实现以(())引起注意，复制具有相同格式/变量名的行，只替换了()和{}并删除了我的注释我不知道我在用下面的代码做什么，但它很有用。



问题：这合法吗？

>译注:Automatic1111 web Ui到今天(2022-10-17)也没有确定他的开源许可证.github有issue也在讨论这个问题.[License? · Issue #24 ](https://github.com/AUTOMATIC1111/stable-diffusion-webui/issues/24)[(IMPORTANT) Add a license to this repository · Issue #2059](https://github.com/AUTOMATIC1111/stable-diffusion-webui/issues/2059)作者虽然说了想使用AGPL协议但是也没有执行![image-20221017120930555](https://picgo-swtt.oss-cn-beijing.aliyuncs.com/image-20221017120930555.png)
>
>所以网上说的NovelAI 违反gpl开源协议并不可靠



**2nd event:** NovelAI在产品上集成了“Hypernetworks”为NovelAI提供了更好的文本生成模块，这些模块用于提示学习(prompt tuning)。根据Novel AI的说法，Hypernetworks与2016年提出的[Hypernetworks]([[1609.09106\] HyperNetworks (arxiv.org)](https://arxiv.org/abs/1609.09106))不同。

问题：这有多少是真实？

你可以在他们的官方声明中看到这一点：https://blog.novelai.net/novelai-improvements-on-stable-diffusion-e10d38db82ac 点击"Hypernetworks" 选项.



**3rd event:** 黑客泄露了NovelAI的“hypernetworks”数据，以及他们最初的NovelAI模型。这是黑客的非法举动。

您可以在这里看到NovelAI对此活动的官方公告： https://twitter.com/novelaiofficial/status/1578529189741080576

![image-20221017122148197](https://picgo-swtt.oss-cn-beijing.aliyuncs.com/image-20221017122148197.png)



**4th event:** 当这一切发生时, [u/AUTOMATIC1111](https://www.reddit.com/u/AUTOMATIC1111/) 在他的AUTOMATIC1111 web ui 中添加了对泄漏数据的支持, 以便与泄漏的NovelAI的"hypernetworks"系统兼容 . 他的观点 [here](https://www.reddit.com/r/StableDiffusion/comments/y1uuvj/comment/is298ix/?utm_source=share&utm_medium=web2x&context=3):

Automatic 最开始实现的hypernetworks 与泄漏的初始化代码之间的比较：

![对比](https://user-images.githubusercontent.com/23345188/194727441-33f5777f-cb20-4abc-b16b-7d04aedb3373.png)

问题：在Automatic1111 web ui上添加此hypernetworks 实现是非法的吗？



**5th event:** Stable AI的人私下指控[u/AUTOMATIC1111](https://www.reddit.com/u/AUTOMATIC1111/) 窃取代码![lu014Ca](https://picgo-swtt.oss-cn-beijing.aliyuncs.com/lu014Ca.png)

AUTOMATIC否认这些指控，并声称NovelAI从一开始就窃取了他的代码

![AUTOMATIC denies these accusationsand makes his own claim that NovelAI stole his code to begin with](https://picgo-swtt.oss-cn-beijing.aliyuncs.com/jgyvup5.png)



**6th event**: Emad含蓄(implicitly )地声称Automatic1111的行为[鼓励了非法获取信息的传播](https://old.reddit.com/r/StableDiffusion/comments/xz4j1p/recent_announcement_from_emad/), 但是 [u/AUTOMATIC1111](https://www.reddit.com/u/AUTOMATIC1111/) [为自己辩护](https://github.com/AUTOMATIC1111/stable-diffusion-webui/issues/1936#issuecomment-1272272599).

<img src="https://picgo-swtt.oss-cn-beijing.aliyuncs.com/11p03u41kns91.jpg" style="zoom: 33%;" />

![image-20221017124404025](https://picgo-swtt.oss-cn-beijing.aliyuncs.com/image-20221017124404025.png)



问题：在Automatic1111 web ui中添加对“Hypernetworks”RNN的支持，会证明禁止web ui本身是正当的吗？

在拒绝删除他最近的更新后，AUTOMATIC立即被Stable Diffusion server ban了

![lu014Ca](https://picgo-swtt.oss-cn-beijing.aliyuncs.com/lu014Ca.png)

问题: Stability AI做的对吗

Please up vote. ***All people must work in this in order to defend what is ours.***



***7th Event:*** Emad,就对[u/AUTOMATIC1111](https://www.reddit.com/u/AUTOMATIC1111/)的行为 [公开道歉](https://github.com/AUTOMATIC1111/stable-diffusion-webui/discussions/2509) 

![image-20221017125852081](https://picgo-swtt.oss-cn-beijing.aliyuncs.com/image-20221017125852081.png)

