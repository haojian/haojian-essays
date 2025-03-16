---
layout: post
title: "价值函数."
description: "human centered value function."
tags: [life, phd, cn]
---


拖了很久，终于在jason的接连催促下，我把 [email++](https://arxiv.org/abs/1907.01423) 上传到了 arXiv。email++ 的想法很简单：如何去修改已经发出去的邮件。因为SMTP protocols的关系，邮件发出去以后，会存储在了收件人的服务器，发件人就不能再修改了。我经常因为蹩脚的语法，发现刚发出去的邮件有时态错误，想修改发出去的邮件。做法也很简单，把邮件里面一部分内容换成图片超链接，而图片是存在第三方服务器上的。这样只要更新第三方图片，收件人看到的邮件也会相应改变。整篇论文介绍了我们的chrome插件，但是没做user study。

<iframe width="560" height="315" src="https://www.youtube.com/embed/HlFFL0eH3sc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
回过头去看，email++ 是我刚入学博士的心态，想在顶级学术会议上证明自己。我想模仿的是 chris harrison 的 [A New Angle on Cheap LCDs](http://chrisharrison.net/projects/obliqueLCD/lcdangle.pdf) 和 juho kim 的 [Content-Aware Kinetic Scrolling for
Supporting Web Page Navigation](https://juhokim.com/files/UIST2014-CAKS.pdf). 我说服自己这是一个很好的锻炼机会，可以练习我的写作，学习怎么样把一个简单而可爱的想法发表。但是我水平不够。这篇论文投了两次 (UIST 2017, CHI 2018), 两次分数都是borderline, reviewers 表示愿意接收这篇论文如果我做一个user study的话。我觉得这篇论文的核心不在于user study。我不想做一个画蛇添足的user study来讨好审稿人。

> 我命硬. 学不来弯腰.        - [Gai 沧海一声笑](https://www.youtube.com/watch?v=06urMzpGxko)

很长一段时间，我对自己感到很失望，因为这一次小实验我没有抓到发表论文的精髓。这个精髓在于很多方面: 想法，执行，以及写作。可能每个地方差一点，导致我最后不能把它发表。一直到有一天看到 david chang 的一个[访问](https://www.wired.com/2016/07/chef-david-chang-on-deliciousness/), 里面有一句话让我“顿悟”。


>To compensate for my lack of dexterity, speed, and technique, I think about food constantly. In fact, I’m much stronger at thinking about food than I am at cooking it.


我想如果我是一个厨师的话，我走的也是david chang的路线。cmu里有很多让人望尘莫及的stellar scientists，他们一路顶级学霸，非常好的数学功底和编程能力。可能我写一天的程序，大佬们坐下来一小时就写完了。写作，性格，工程能力，我肯定不是最好的执行者。这些局限迫使我要去想更多。事实上，我对每个项目想的时间要比做的时间多很多。时间久了，我反而觉得这种局限是一种特别的优点。有点像Frank Lloyd Wright设计fallingwater时，压低了窗口处天花板的高度，为了促使住户看向窗外的景色。


<img src="/resources/fallingwater_ceiling.jpg" width="700px" alt="fallingwater"/>
 <i>Fallingwater 是一座建筑史上特别有名的住宅, 建立在匹兹堡附近的一处瀑布旁边。Frank Lloyd Wright 在设计这座住宅时，提倡了一种不同的建筑理念：住宅要完全融入自然之中。每个房间靠近窗口处的天花板都会拉低，强迫房间里的人看向窗外的自然环境。</i>


当我开始看更大更远的地方的时候，我就开始觉得email++这篇论文有些不值得我的时间，所以我最后决定不在这个项目上继续投入时间。几乎在同一时间，我砍掉了好几个就是为了证明自己的论文项目。


>悟已往之不谏，知来者之可追。
实迷途其未远，觉今是而昨非。
舟遥遥以轻飏，风飘飘而吹衣。
问征夫以前路，恨晨光之熹微。

当我开始看更大更远的地方的时候，


即便我浪费了很多时间在电影和游戏上。


以至于我觉得不应该再花任何时间在这个项目上。


我想要去看更远的地方。
[Xiaodi Hou](http://www.houxiaodi.com/) 有一句话让我印象很深刻。大意是很多大公司工程师们一天写完的东西，我可能要一星期才能写完，但是我一年写出来的东西，那些工程师可能永远写不出来。
[The Innovator's Dilemma](https://www.amazon.com/Innovators-Dilemma-Revolutionary-Change-Business/dp/0062060244) 里也有





可能我

想明白这件事以后，我开始比以前更加义正言辞地看闲书了。匹兹堡是一个很适合读书的地方，如果我没有被电脑游戏吸引过去的话。



我是一个很喜欢价值函数(value function)的人，回想起来，我的大部分论文里面都会把一个实际问题变成一个价值函数，然后去优化它，寻找最优解。

tracko 优化的是distance ressidual
elasticplay 里我定义了一个concept叫，优化的是 
wish 优化的是 shape ressidual。
microwave oven 优化的是heating residual。

这件事的起因可能是来自于16年当时我开始对machine learning fairness 感兴趣的时候，和dawei yin的讨论。从hci的角度来看，我觉得这个是一个非常有意思的问题，但是dawei也觉得这个挺有意思，显然没有我那么激动。他把这个东西描述成 另外一个value function。对他而言，他们的任务并没有任何区别，只要是有一个value function，他们就可以提供最好的办法来优化他。这让我觉得这个问题最后可能更多是hci问题，如何去定义这个价值函数。但是dawei 当是这段话给了我很大的启示，所以之后几年没当我不知道怎么解决这个问题，我就把这个问题变成一个价值函数，然后去优化他，这也成了我研究里面的一个signature。

上周六和hcii的phd去吃巴西烤肉自助，我想我终于到了一个年纪不能再费力得吃了。自助是让人感觉self fullfiling的事情，因为当你觉得你吃回票价了，你觉得完成了一个很重要的任务，他既有翻山越岭的酣畅感，又有击败对手的成就感。value function就是吃了多少价值的东西。在hci读了几年phd，我终于把value function改成了 human centered value function. it's not about the value i have consumped, it's about how happy i would be. my happiness is based on a combination of how much i have consumed, whether i have beaten the restaruant, and how comfortable i would be after that meal. 

这件事让我想起来前一阵子看到的andrew yang的human centered economy，虽然andrew yang 并不是一个scholar，但是我非常appreciate 他的reflection。社会从计划经济，到市场经济，再到社会主义最后的按需非配。但是大家其实并不是完全trust每个人的需求。因为穷有穷活法，富有富活法。按需分配的基础是在于每个人的需求。我觉得human centered economy 是一个很好的transition，between the market economy and the ultimate utopia of socialism。optimization 是一个很有意思的问题，是因为他从来基于一个资源不足的假设。而追求gdp 发展的

在早期社会，社会的optimization里面，是追求总资源的增加，而过了一定阶段以后，就应该变成质量的增加，或者是营养的吸收率，这里的第一步metric 需要发生变化，就是human centered metrics。
elasticplay里面，maximize the human perception。我们希望用户花最多的时间在这个视频浏览上。然而更好的办法，

人们总说选择要比努力要重要，大家总是喜欢用一个四象限的图来表示选择的方向。这是一个retrospective的看法。因为只有上帝视角才能看到你要走的方向。一个更真实的方向是 human-centered value function。今年我又去了glasgow，感谢老板的funding，我又没有论文去了chi。在chi我看到很多work，我发现我下意思地把work 分成四类。matrix

第一类是，特别后悔自己没做出来的。感觉自己已经那么接近了，但是我却错过了。比如equal opportunity，比如word embeding for implicit bias，比如icml那篇lasting impact，这些work我是有skill却做的，而且我也已经很接近了，但是我却没做到。

第二类是，谢谢你完成了这个work，那些work我觉得很有意思，但是我不具备这样的skill来完成这个task，你真厉害.

第三类是，你的work真有意思，虽然我有时间有技能也不一定会去做这个项目，但是我非常尊敬和欣赏你的work。

第四类，是剩下的work。有些工作我并不赞同他们的position，或者设计。


