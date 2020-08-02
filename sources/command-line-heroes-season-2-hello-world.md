[#]: collector: (bestony)
[#]: translator: ( guevaraya)
[#]: reviewer: ( )
[#]: publisher: ( )
[#]: url: ( )
[#]: subject: (Command Line Heroes: Season 2: Hello, World)
[#]: via: (https://www.redhat.com/en/command-line-heroes/season-2/hello-world)
[#]: author: (RedHat https://www.redhat.com/en/command-line-heroes)

代码英雄 第二讲：你好，世界
======
**00:07** - _多人发声_

你好，世界。

**00:12** -_沙隆·伊特巴雷克(Saron Yitbarek)_

你好 世界。这是信号还是噪音？我们日日夜夜无休止编码和压测的工作，最终回到一个问题我们获取到是信号吗？

**00:29** - _多人发声_

你好

**00:29** - _沙隆·伊特巴雷克(Saron Yitbarek)_

或者我们的信号是不是丢了？我们一直在制造噪音？

**00:40** - _沙隆·伊特巴雷克(Saron Yitbarek)_

我是沙隆·伊特巴雷克(Saron Yitbarek)，这是代码英雄第二讲，来自红帽原创播客。我们已经在译文中看到今天的节目。都是关于编程语言：他们是怎么来的，如何选择其中一个语言来学习。我们深入研究如何与机器对话。这些语言是如何演化的。以及我们如何用他们使我们的作品优美。

**01:08** - _萨瑞（Sari）_

黛西，黛西，来告诉我你的正确回答。

**01:11** - _沙隆·伊特巴雷克(Saron Yitbarek)_

如果你像我一样是一个开发者，你可能觉得精通多种语言的人很难。优秀点你可能知道Java，Python，Go JavaScript，Node，最差也得要熟悉 C++ 吧。可能你为了生计熟悉经典语言 COBOL。甚至可能你是一个菜鸟，像达尔特（Dart）一样。。。 编程语言太繁多了。

**01:36** - _沙隆·伊特巴雷克(Saron Yitbarek)_

奇怪的是，我们正在讨论的计算机只讲一种语言：机器语言。所有这些 1 和 0 都是以二进制形式飘过。归根结底，我们学习的每个语言都是殊途同归。不管有多抽象，它都是用来简化我们的工作。

**02:03** - _沙隆·伊特巴雷克(Saron Yitbarek)_

这就是我希望你们在故事开讲之前始终记住，因为从这一刻开始，经典辉煌的这一刻，一个妇女说到：“你知道么？我是人类，我不想用二进制讨论，不想用二进制思考，我就想用英语文字去编程。”

**02:22** - _沙隆·伊特巴雷克(Saron Yitbarek)_

在今天可能看来是一个简单易于接受的概念，但曾几何时，使用人类的方式与计算机对话的这个主意说轻点是一个笑话，严重点就是亵渎。

**02:37** - _沙隆·伊特巴雷克(Saron Yitbarek)_

代码英雄第二讲是关于支撑我们做事情的螺钉螺母。这一讲的的英雄是一个女主人公，如果你想更深一步的理解我们的实际状况，我们需要了解她的经历。因此给你们介绍：软件第一夫人。

**02:58** - _人物5_

尊敬的先生们和女士们，我非常荣幸的给你们介绍格雷斯·玛丽·哈伯准将，谢谢您。

**03:02** - _格雷斯·哈伯(Grace Hopper)_

我曾到加拿大的圭尔夫大学演讲，我必须在多伦多的机场办理入境手续。我把护照递给移民官，他打量了护照和我说：“你是做什么的？”

**03:17** - _格雷斯·哈伯(Grace Hopper)_

And I said, "United States Navy."
然后我说，“美国海军”

**03:20** - _格雷斯·哈伯(Grace Hopper)_

她再次深深的打量我一下。然后他说:"你一定是海军里最老的。"

**03:28** - _沙隆·伊特巴雷克(Saron Yitbarek)_
他就是1985年的海军少将格雷斯·哈伯(Grace Hopper)。当时她79岁在麻省理工学院发表了著名的演讲。可以说，她是一个传奇人物。她是机器无关独立编程语言之父，她当年通过编译器用人类语言替代数学符号编程。

**03:51** - _沙隆·伊特巴雷克(Saron Yitbarek)_

她获得了国家技术奖章，她死后，追授国家自由勋章。因此：可不是瞎说，他们称她“令人称奇的格雷斯”。

**04:03** - _克莱尔·埃文斯(Claire Evans)_

如果有人生来就是计算机程序员，那它就是格雷斯。

**04:06** - _沙隆·伊特巴雷克(Saron Yitbarek)_

这是克莱尔·埃文斯(Claire Evans)，一个科技记者和《宽带》的作者，而这本书讲述了科技领域的先锋女性。埃文斯描绘了早期的计算机世界，格雷斯·哈伯(Grace Hopper)在1940年作为年轻的女性进入了美军的海军预备役部队，而当时的电脑就是一个小房子。

**04:25** - _克莱尔·埃文斯(Claire Evans)_

所有那些早期程序员，他们像个牧师，他们是一群擅长枯燥乏味的做事情，因为那会没有编译器，没有编程语言，人们是确实是一个比特一个比特的机器编程。

**04:42** - _克莱尔·埃文斯(Claire Evans)_

为了持续的做好这类事情，你真的必须是一个特别的人，而格雷斯真的就是那种人。

**04:49** - _沙隆·伊特巴雷克(Saron Yitbarek)_

现在，她意识到限制人类使用机器语言是多么的疯狂。就像走路的时候去告诉你身体的每个原子该怎么做。这是可能的吗？是，效率呢？不高。

**05:06** - _沙隆·伊特巴雷克(Saron Yitbarek)_

这需要在程序员的意图和计算机的动作之间选一个捷径。自从有了算盘，人类一直用机械式的数学思维，他们就按部就班的在计算机上选择这样的路径。

**05:19** - _克莱尔·埃文斯(Claire Evans)_

在过去，数学家常常必须做出所有的数学演算。所有这些枯燥的一步一步的工作都是为了得到一个真实的有趣的答案。然后有了计算机后，它尽可能的承担了这些机器运算，所以解放了数学家去高级的，更智慧的，系统性的操作。

**05:39** - _克莱尔·埃文斯(Claire Evans)_

实际上，当时没有什么变化。最终，有了计算机，数学家必须变成一个程序员。然后他们为了一点运算而去写代码，受困于所有这些枯燥的面向过程的比特流。

**05:53** - _克莱尔·埃文斯(Claire Evans)_

因此，我认为，格雷斯的预想是她希望计算机能够辅助数学家然后他们可以去更伟大的去思考，没有被枯燥繁琐的事情困扰去做更伟大的事情。

**06:12** - _沙隆·伊特巴雷克(Saron Yitbarek)_

哈伯也加入了思想家的行列。我们都知道，帕斯卡（Pascal）在17世纪发明了第一台计算器。巴比奇在19世纪发明了分析引擎。这些伟大的杰作是发明家们想解放人类的大脑而造的。这些发明让我们处理数据的能力空前绝后。这就是格雷斯哈伯在发明了所有人认为不可能的东西后，就理所当然的进入思想家的行列。

**06:42** - _克莱尔·埃文斯(Claire Evans)_

我觉得，哈伯的想法是人们应该用人类语言与计算机沟通，这个语言必须独立于机器，因此在不同计算机之前的交互操作在当时引发了一场变革。

**06:59** - _克莱尔·埃文斯(Claire Evans)_

早期她称这个为 “自动化编程”的概念，而支持她的人们被看作是程序员和计算机从业人员的里的太空学员。

**07:12** - _克莱尔·埃文斯(Claire Evans)_

而那些迟迟不上岸的人们被看成了尼安德特人，这在当时是计算机界的一个巨大的分歧。

**07:21** - _沙隆·伊特巴雷克(Saron Yitbarek)_

哈伯很难轻易的说服他的主管去跳过这个分歧。但他的责任就是去尝试。

**07:30** - _格雷斯·哈伯(Grace Hopper)_

当然总有人在后面排队。排队意味着你的老板迟早会相信。现在你跳过它，你就得不到预算。因此你有双重责任走这条路：不要跳过，不断的说服你的老板让你你不断前进和探索，你会进一步拥有未来。

**07:52** - _沙隆·伊特巴雷克(Saron Yitbarek)_

她推动的未来就是我们的现在。几乎你和我依赖的每一个种语言都归功于哈伯和她第一个编译器。因此太空学员活了下来，尼安德特人灭亡了。

**08:07** - _沙隆·伊特巴雷克(Saron Yitbarek)_

写代码不用数字，用人类风格的语言是她的观点。你正在敲下“执行操作 8”，或“关闭 文件 C”的精简操作，这才是符合人类习惯的编程。

**08:21** - _克莱尔·埃文斯(Claire Evans)_

格雷斯的特别想法是计算机将改变世界，但是没有人知道如何接触到计算机并使用它，那么世界也就不会改变。因此她希望一定要开放才能让尽可能多的人用，要易于交互才能有更多的人接触到。

**08:37** - _克莱尔·埃文斯(Claire Evans)_

这就需要编程在可理解行和可读性上做一些妥协。因此最终创造一个编程语言的目标就是给机器提供更多切入点，把它从神坛拿下来，让它开发的面向大众和未来新一代。

**08:59** - _沙隆·伊特巴雷克(Saron Yitbarek)_

我想在这里打断并强调下克莱尔的说法：现在我们所已知的编程语言都来源于科技开放的先驱。是从数学博士的神探拿下来的，它让编程开发更容易。

**09:14** - _沙隆·伊特巴雷克(Saron Yitbarek)_

The spirit of the compiler that does all that work, it's motivated by a sense of empathy and understanding.
编译器的本质是做所有解释性和理解性目的的工作。

**09:21** - _沙隆·伊特巴雷克(Saron Yitbarek)_

克莱尔有一个观点关于为什么哈伯是推动变革的唯一妇女。在于在二战期间不得不做哈伯的工作。

**09:29** - _克莱尔·埃文斯(Claire Evans)_

她的工作是解决扫雷，导弹测试问题和海洋问题。她用所有不同的，交叉的学科模拟战争里的所有的暴力，混乱和现实的灾难，将他们转化成在 Mark I 计算机上运行的程序。

**09:45** - _克莱尔·埃文斯(Claire Evans)_

她知道如何在语言之间去做翻译转换。我的意思不是说计算机语言，意思是人类语言。她精通如何倾听人类描述复杂问题，并尝试理解问题的背景，其约束信息和所涉及的专业规律，然后将这些转为计算机可以理解的程序。

**10:06** - _克莱尔·埃文斯(Claire Evans)_

从这个角度看她如同早期的编译器。就像一个人类内置的编译器，因为她知道你必须从人类的层次满足人的需求。

**10:17** - _沙隆·伊特巴雷克(Saron Yitbarek)_

编译器就是一个解释和理解的过程。我觉得我们应该在学习新语言或想知道为什么有一些东西根本不能编译的时候牢记这个理念。编译器的工作就是满足你生活种使用的语言。

**10:32** - _沙隆·伊特巴雷克(Saron Yitbarek)_

格雷斯·哈伯知道人类一旦可以学着去将编程语言，一旦编译器可以将我们的意图转换为机器语言，就像洪水大门打开一样。

**10:43** - _克莱尔·埃文斯(Claire Evans)_

她知道如果计算机太孤立和太具体的话，就不会发展为一个产业，成为改变世界的力量。也就是说计算机的从业者不能与在机器上问题要解决的人直接沟通。

**11:00** - _克莱尔·埃文斯(Claire Evans)_

因此她真的是一个善于人类语言翻译的专家，我是认为的，是的，这使她有独一无二的机会去思考和创建编程语言。

**11:15** - _沙隆·伊特巴雷克(Saron Yitbarek)_

哈伯的工作是将英文数据的加工语言最终演变为 COBOL 语言，它是接近完美的语言，因为它不浮华，很适合商务用途，格雷斯·哈伯也是这样的人。

**11:28** - _沙隆·伊特巴雷克(Saron Yitbarek)_

从某种角度看，她给了我们一个很像她的语言。像哈伯一样，BOBOL 语言也很长寿。她现在已经60多高寿了。

**11:50** - _沙隆·伊特巴雷克(Saron Yitbarek)_

格雷斯·哈伯的编译器就像一个巴别鱼，吸收编程人员和机器之前的信号含义。然后他们从最高级的抽象翻译这些事务。

**12:03** - _沙隆·伊特巴雷克(Saron Yitbarek)_

接着，大约10年之后，我们又有了另一个重要的思潮在语言界兴起。想象下画面是这样：自由软件社区在1980年出现，但是 Unix 的替代 GNU 被造出来后却没有开放和自由的编译器随之出现。

**12:22** - _沙隆·伊特巴雷克(Saron Yitbarek)_

为了让 GNU 给我们一个彻底的UNIX开源来替代品，为了让编程语言在开源世界蓬勃发展，社区需要找来格蕾丝·哈勃-我们需要一个开源编译器。

**12:38** - _沙隆·伊特巴雷克(Saron Yitbarek)_

这是兰登·维特，红帽的平台架构师，来讲讲他对这个事情的理解。

**12:45** - _兰登·维特(Langdon White)_

在80年代，你可能轻轻松松在编译器上花费一万块钱。免费是最大的问题。我没有多余的钱去给自己买编译器。再一个事实我又必须为所有我想要的目标平台自讨腰包买一个对应的编译器。因此，这些天主要在用Unix，但又是不通的发行版。

**13:06** - _兰登·维特(Langdon White)_

因此你做不到只买一个，你需要为不同的架构，不同的供应商购买多个编译器。

**13:14** - _沙隆·伊特巴雷克(Saron Yitbarek)_

兰登指出这不仅仅是成本问题，在一些情况下，对编码工作带来问题。

**13:21** - _兰登·维特(Langdon White)_

大家都没有意识到用很特定的方法构思你的代码是一个大问题。仅在编译器上执行 for 循环的嵌套，或执行 while 循环的嵌套或者类似的事情都没问题。

**13:38** - _兰登·维特(Langdon White)_

因此，大家都了解，如果你不知道编译是如何优化你的代码，那么如何写出最优的代码对你将更难。

**13:49** - _沙隆·伊特巴雷克(Saron Yitbarek)_

必须要提的是，我们需要一个可免费的，可获得的，可值得信赖的编译器。就是我们需要的 GNU C 语言编译器，GCC。它是最好的，首版本《野兽》1987年发布，当时格蕾丝·哈勃的编译器革命和自由软件运动结合物。

**14:12** - _沙隆·伊特巴雷克(Saron Yitbarek)_

It standardized things and let everybody compile what anybody else had written. The richness of our languages is thanks to that moment.
它是使编译标准化从而让所有人可以编译别人写的代码。我们丰富多彩的编程语言多亏了这个事件。

**14:22** - _卡罗尔·威灵(Carol Willing)_

The fact that the GCC was open sort of moved languages to a different level.

**14:29** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Carol Willing works at Project Jupiter, and she's the former director of the Python Software Foundation.

**14:35** - _卡罗尔·威灵(Carol Willing)_

People started realizing that proprietary languages, while they served a purpose at the time, they weren't going to gain the acceptance and adoration of the developer community. Because if I'm a developer, I'm going to want to learn what is most commonly used and as well as what is new and on the forefront.

**14:59** - _卡罗尔·威灵(Carol Willing)_

I don't necessarily want to develop a skill that will lock me into one technology. I think one of the reasons that Python was so successful is it was open source, it had a very clean syntax.

**15:11** - _卡罗尔·威灵(Carol Willing)_

What it was doing is it was allowing people in a common way to solve problems quickly, efficiently. And to also allow people to collaborate. And I think those are the signs of good programs and good libraries is: if you can get your work done with a minimum amount of headache and you can share it with others. I think that's golden.

**15:35** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Over the years, the GCC evolved to support Java, C++, Ada, Fortran, I could go on.

**15:43** - _卡罗尔·威灵(Carol Willing)_

By having a common underlying interface like the GCC, it lets people take languages and then customize them to their particular needs. For example, in the Python world, there's many different libraries and even specifically in the scientific Python world, we've got things like numpy, and scikit-image, scikit-learn.

**16:08** - _卡罗尔·威灵(Carol Willing)_

And each of those had sort of a more specific task that they are known for. So, we've also seen things like bioinformatics and natural language processing. And so people are able to do many different things working off a common base. But then putting elements into their languages or libraries that allow them to optimize problem solving in their particular industry or area.

**16:42** - _沙隆·伊特巴雷克(Saron Yitbarek)_

So, this is what happens when compiler technology runs headfirst into the open source movement, right? Over time, the collision creates a big bang of new community-supported languages that anybody can learn and build with.

**16:58** - _沙隆·伊特巴雷克(Saron Yitbarek)_

There are hundreds and hundreds of those languages being used today.

**17:03** - _卡罗尔·威灵(Carol Willing)_

As open source became more popular and more accepted, what we've seen is a proliferation of languages. There are a number of languages around cell phone technology and mobile. Different languages that help make game development more straightforward. All purpose languages, like Python and Ruby that were sort of foundational for the web development and delivery of web applications and websites.

**17:34** - _沙隆·伊特巴雷克(Saron Yitbarek)_

The list goes on. And, yeah, that Tower of Babel we're building is just going to get more packed in the future. But look, you can also see it as a cornucopia, a language feast. And we're going to help you sort through that feast — next.

**17:55** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Okay, so I know where the language flood came from. But how do we make sense of it all? How do we pick out languages that matter to us? It's a big question, so I brought in some help: _克雷夫·汤普森(Clive Thompson)_'s one of the best writers out there for making sense of the tech world. He's a columnist at Wired, a contributing writer at the New York Times Magazine, and he's working on a book now about the psychology of computer programmers.

**18:24** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Which is perfect, because we need to know what's going on in our brains when we choose which ones to learn.

**18:31** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Here's me and Clive hashing it all out.

**18:35** - _沙隆·伊特巴雷克(Saron Yitbarek)_

When I was first starting out as a new developer, I just said, "Lemme find the best one, I'm going to get really good at it. And then I'll be done."

**18:44** - _沙隆·伊特巴雷克(Saron Yitbarek)_

But it's not quite that simple. Why are there so many programming languages?

**18:49** - _克雷夫·汤普森(Clive Thompson)_

Each language has sort of a bias of things that it's good at. So, typically, the reason that someone creates a new language is there's something they want to do that existing languages aren't good for. JavaScript is a good example of that.

**19:03** - _克雷夫·汤普森(Clive Thompson)_

Netscape had created a browser back in the mid '90s and all these web masters wanted to do something a little more interactive. They wanted there to be a way to have a bit of scripting inside their website.

**19:16** - _克雷夫·汤普森(Clive Thompson)_

And so these demands were coming to Netscape. And they were like, "Alright, we need, there's nothing out there that can do this, we need a scripting language that we build inside our browser."

**19:25** - _克雷夫·汤普森(Clive Thompson)_

And so they hired Brendan Eich, who was considered a senior guy. He was like 32, and everyone else was like 21.

**19:32** - _沙隆·伊特巴雷克(Saron Yitbarek)_

That's senior in developer world.

**19:35** - _克雷夫·汤普森(Clive Thompson)_

And they gave him ten days to make JavaScript. So he literally just didn't sleep for ten days and he frantically cranked out a scripting language. And it was kind of ungainly and kind of a mess. But it worked. And it allowed people to do very simple things, it had buttons and dialogs and popups and whatnots.

**19:54** - _克雷夫·汤普森(Clive Thompson)_

And so that's an example of a language that came, was created to do something that wasn't really possible at that point in time.

**20:01** - _沙隆·伊特巴雷克(Saron Yitbarek)_

That's fascinating.

**20:03** - _克雷夫·汤普森(Clive Thompson)_

So that's why so many languages exist, is that people keep on finding a reason to do something that no one else can do.

**20:11** - _沙隆·伊特巴雷克(Saron Yitbarek)_

So what is so interesting to me about the relationship between developers and our programming languages is we have such a strong attachment to these tools, why is that?

**20:22** - _克雷夫·汤普森(Clive Thompson)_

There's a couple reasons why. One is that sometimes it's literally just an accident of what was the first language that you learned. And it's kind of like your first love.

**20:30** - _克雷夫·汤普森(Clive Thompson)_

And I think it's also like different personalities work with different types of languages. Like, you look at Facebook, and it was designed using PHP. And PHP is kind of a hairball of a language. It's very irregular. And it sort of grew in these fits and starts. And that's sort of the way Facebook feels, too.

**20:49** - _克雷夫·汤普森(Clive Thompson)_

In comparison, the guys at Google decided, "We want a super high performance language, because Google, at Google we're all about things running really fast, and things, sustaining trillions of users at once."

**21:02** - _克雷夫·汤普森(Clive Thompson)_

And so they decide to make Go, and Go is a really terrific language for that sort of high-performance computing.

**21:08** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Let's go a little bit deeper. Is it that I, as a developer, with my specific personality, am going to be naturally attracted to certain languages? Or that the language I work in might influence my personality?

**21:25** - _克雷夫·汤普森(Clive Thompson)_

Well, definitely both. But I do think that there is a really strong resonance that people find when they hit a language that they like. You go to a computer science curriculum and you sort of learn what you have to learn: they're all teaching Java. Sometimes more JavaScript or Python.

**21:46** - _克雷夫·汤普森(Clive Thompson)_

But the point is, you're forced to learn it, so you learn it. But what do people do when they have the choice? And this is where you really see how the sort of emotional or psychological style of someone gravitates towards a language, because I talked to one guy who tried learning JavaScript a bunch.

**22:03** - _克雷夫·汤普森(Clive Thompson)_

And it was just sort of, it's kind of an ugly language to look at. It's go the curly bracket nightmare going on. And so he tried and failed and tried and failed and tried and failed. And then one day he saw a friend working in Python. And it just looked so clean and beautiful to him. He was kind of a writer, and it's often regarded as a writerly type of a language, because the indentation makes everything easy to read.

**22:28** - _克雷夫·汤普森(Clive Thompson)_

And it just clicked with him, because there was just something about the way that Python worked and looked, it's beautiful sparseness, that hit him.

**22:39** - _沙隆·伊特巴雷克(Saron Yitbarek)_

So, talking with Clive I realized there are languages that are thrust upon us. I'm talking about those ancient languages that are just baked into everything we work with — the code Latin.

**22:53** - _沙隆·伊特巴雷克(Saron Yitbarek)_

But there're also languages we choose, the languages that fit our personalities. And if you want to know what's new and shaking things up, you want to ask a developer what they use on the weekend.

**23:05** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Here's more of our conversation:

**23:08** - _克雷夫·汤普森(Clive Thompson)_

So when I ask people: "What are you doing in your spare time?" It'll be all this weird stuff. I think it's actually one of the things that sort of, you know, nice and laudatory about developer behavior is that they tend to be very curious people.

**23:22** - _克雷夫·汤普森(Clive Thompson)_

I know people that decided, "I'm going to learn Erlang, just for the hell of it."

**23:26** - _沙隆·伊特巴雷克(Saron Yitbarek)_

I'm trying to imagine these projects that people are working on on the weekends. And it's almost like the project is secondary. It's like the learning of the tool, the language, is more important. That's really what they're there for.

**23:41** - _克雷夫·汤普森(Clive Thompson)_

Exactly. This, is sort of why you'll see people just constantly re-iterating over and over again these calendaring and to-do list things because it's a very quick way, just to figure out, yeah, what does this language do and how does it work and it almost doesn't matter what I'm building, so long as I'm building something.

**23:56** - _克雷夫·汤普森(Clive Thompson)_

They want to know what it feels like to think in that language. Is it going to be, is it going to feel easy, and thrilling and fluent in a way that I'm not experiencing with the current languages? Is it going to open up doors to make things easier to do?

**24:13** - _克雷夫·汤普森(Clive Thompson)_

So there's a possibility space that occurs when you encounter a new language that can be really exciting. Imaginatively exciting.

**24:20** - _沙隆·伊特巴雷克(Saron Yitbarek)_

So I'm a Ruby, a very proud Ruby on Rails developer, I think it was about two years ago that another pretty well known Ruby developer, Justin Serrals, did this really great talk advocating for this idea that a language doesn't need to be sexy to be used.

**24:41** - _沙隆·伊特巴雷克(Saron Yitbarek)_

And his thesis, his whole point was that Ruby was really exciting because it was new. And it kind of got to a point about a couple years ago where it just didn't need any more things. It was done. It was a stable language, it was a mature language, and, as a result of it being mature, it's not as exciting for developers. It's not this new toy to play, and so we kind of slowly moved away from it on to the next shiny thing.

**25:05** - _沙隆·伊特巴雷克(Saron Yitbarek)_

So, in a sense, it's almost our own curiosity that might kill a language, or make it a little more stale, independent of whether the language is actually good or bad.

**25:18** - _克雷夫·汤普森(Clive Thompson)_

I think that's absolutely true. In fact, the downside of this deep curiosity and desire to self-educate that you see amongst developers is that they're constantly trying to find the new shiny thing. And use that language to replicate things that are already basically done pretty well by other languages.

**25:37** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Right.

**25:37** - _克雷夫·汤普森(Clive Thompson)_

So that's that. Curiosity is a benefit and a trap.

**25:43** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Yeah, beautifully put.

**25:49** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Sometimes our curiosity may be a trap. But it's also the thing that fuels the evolution of languages. Every new language is created because someone said, "What if?" They come about because that developer wanted to do something different.

**26:06** - _沙隆·伊特巴雷克(Saron Yitbarek)_

They wanted a whole new way of saying it.

**26:08** - _格雷斯·哈伯(Grace Hopper)_

And I'll promise you something.

**26:11** - _沙隆·伊特巴雷克(Saron Yitbarek)_

I think Grace Hopper deserves a last word here.

**26:15** - _格雷斯·哈伯(Grace Hopper)_

Just during the next 12 months, any one of you says that we've always done it that way, I will instantly materialize beside you and I will haunt for 24-hours. And see if I can get you to take another look. We can no longer afford that phrase, it's a dangerous one.

**26:34** - _沙隆·伊特巴雷克(Saron Yitbarek)_

The story of Grace Hopper and the first compiler reminds us that there's always a better way to do something if we can just find the words.

**26:43** - _沙隆·伊特巴雷克(Saron Yitbarek)_

And, no matter how abstract those languages become, whether we're floating high or low over the ones and zeroes of machine language, we need to make sure it's a smart choice. We choose the language, or maybe even build the language that helps our intentions come closer to reality.

**27:03** - _沙隆·伊特巴雷克(Saron Yitbarek)_

If you want to learn more about languages and compilers, you are not alone. We pulled together some super useful material to help you dive deeper. And it's all waiting for you in our show notes. Check it out at redhat.com/commandlineheroes.

**27:20** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Next episode, we're tracking the complicated path toward making open-source contributions. What are the real life struggles of maintainers? How do we make that very first pull request?

**27:32** - _沙隆·伊特巴雷克(Saron Yitbarek)_

We're taking you through Contributing 101.

**27:39** - _沙隆·伊特巴雷克(Saron Yitbarek)_

Command Line Heroes is an original podcast from Red Hat. Listen for free on Apple Podcasts, Google Podcasts, or wherever you do your thing.

**27:48** - _沙隆·伊特巴雷克(Saron Yitbarek)_

I'm Saron Yitbarek, until next time keep on coding.

--------------------------------------------------------------------------------

via: https://www.redhat.com/en/command-line-heroes/season-2/hello-world

作者：[Red Hat][a]
选题：[bestony][b]
译者：[译者ID](https://github.com/译者ID)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCRH](https://github.com/LCTT/LCRH) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出
[a]: https://www.redhat.com/en/command-line-heroes
[b]: https://github.com/bestony
