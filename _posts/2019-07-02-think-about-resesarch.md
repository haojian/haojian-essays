---
layout: post
title: "想."
description: "I’m much stronger at thinking about research than I am at doing it."
tags: [life, phd, cn]
---


拖了很久，终于把 [email++](https://arxiv.org/abs/1907.01423) 上传到了 arXiv。email++ 的想法很简单：如何去修改已经发出去的邮件。因为SMTP protocols的关系，邮件发出去以后，会存储在了收件人的服务器，发件人就不能再修改。我因为蹩脚的语法，经常发现刚发出去的邮件有时态错误，想修改已经发出去的邮件。做法也很简单，把邮件里面一部分内容换成图片超链接，而图片是存在第三方服务器上的。这样只要更新第三方图片，收件人看到的邮件也会相应改变。整篇论文介绍了我们的chrome插件，但是没做user study。

<iframe width="560" height="315" src="https://www.youtube.com/embed/HlFFL0eH3sc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
回过头去看，email++ 是我刚入学博士的心态，想在顶级学术会议上证明自己。我想模仿的是 chris harrison 的 [A New Angle on Cheap LCDs](http://chrisharrison.net/projects/obliqueLCD/lcdangle.pdf) 和 juho kim 的 [Content-Aware Kinetic Scrolling for
Supporting Web Page Navigation](https://juhokim.com/files/UIST2014-CAKS.pdf). 我说服自己这是一个很好的锻炼机会，可以练习写作，学习怎么样把一个简单而可爱的想法发表。这篇论文投了两次 (UIST 2017, CHI 2018), 两次分数都是borderline, 两次审稿意见都是希望我去做一个user study。我觉得这篇论文的核心不在于user study，就不想画蛇添足来讨好审稿人。

> 我命硬. 学不来弯腰.        - [Gai 沧海一声笑](https://www.youtube.com/watch?v=06urMzpGxko)

不管怎样，我对自己感到很失望，因为这一次小实验我没有抓到发表论文的精髓。这个精髓在于很多方面: 想法，执行，以及写作。可能每个地方差一点，导致我最后不能把它发表。一直到有一天看到 david chang 的一个[访问](https://www.wired.com/2016/07/chef-david-chang-on-deliciousness/)。david chang 是一个厨艺界的明星，做过几个很有名的美食纪录片(如The Mind of a Chef)。他谦虚说自己做饭的技巧很差，为了弥补技巧上得不足，他需要不停地去思考食物的可能性。


>To compensate for my lack of dexterity, speed, and technique, I think about food constantly. In fact, I’m much stronger at thinking about food than I am at cooking it. - [David Chang’s Unified Theory of Deliciousness](https://www.wired.com/2016/07/chef-david-chang-on-deliciousness/)


因为这句话，我成了david chang的小粉丝。研究和做饭很像。学校里有很多天赋异禀的stellar scientists，他们一路顶级学霸，非常好的数学功底和编程能力，就像那些手指灵巧的厨师。可能我写一天的程序，大佬们坐下来一小时就写完了。相比于他们，我觉得我的特长是在“想”这件事上。我很喜欢匹兹堡，因为大部分时间都很安静，有大把的时间来读书和空想。实际上，我对每个项目想的时间要比做的时间多很多。时间久了，我觉得这种局限是一种特别的优点。


17年底的时候，我觉得email++这篇论文不值得我的时间，于是决定不在这个项目上继续投入任何时间。<b>并不是我再不需要证明自己，而是我觉得发这些论文也证明不了自己。</b>这篇essay记录了自己这几年的变化: 神棍-》工程师-》高立意低视角，这些变化其实并不是顺序发生，只是类似的事情重复发生，我今天回过头去看，才觉得这是我想要的研究风格。

#### 1. 神棍

有一句玩笑说：“当科学家快要攀登到真理的顶峰时，他们发现神/佛/哲学家已经在那里等候多时了”。我没攀上高峰，在山脚下就遇到了他们。16年读得最有意思的书应该是 Michael Sandel 的 [What Money Can't Buy: The Moral Limits of Markets](https://www.amazon.com/What-Money-Cant-Buy-Markets-ebook/dp/B00633PFQC)。差不多同一时间，[scott klemmer](https://d.ucsd.edu/srk/) 来hcii给talk，一起吃了一顿午饭。Scott 安利了达赖的鸡汤书 [The Art of Happiness](https://www.amazon.com/Art-Happiness-10th-Anniversary-Handbook-ebook/dp/B002UK6NO0)。这几本书带给我两个问题，应该是我的青年危机(Quarter-life crisis)。
<ul><li>“我为什么在这里读博士?”</li><li>“Privacy 为什么重要?”</li></ul>


<img src="/resources/phd_self_expect.gif" width="700px" alt="fallingwater"/>
PhD comics 有这么一张图，描述了每个Ph.D.从入学到毕业的期望。一开始大家都是野心勃勃的博士生，渐渐被导师和审稿人打击，然后最后想着毕业就好。一开始，我和这根单调递减曲线的抗争就是吹牛皮，吹最大的牛皮。一帮博士生半夜在办公室里群魔乱舞，轮番吹牛，午夜夸夸群，描述自己的研究想法对这个世界将产生如何深远的影响。人性，宇宙，怎么宏大怎么来。看问题，时间维度是百年，空间维度是银河系，谷歌这个级别弹指间灰飞烟灭。


现在打开overleaf，还能看到那个时期的好几个论文草稿，其中有一个是研究输入法和人类语言演变的关系。我觉得输入法的自动提示和修改会对每个用户的词汇量产生影响。用户会越来越少打第二页的词组，而很多词汇和单词如果不经常用就会慢慢忘记。以中文为例，我们从手写到打字，从五笔到拼音，算下来也就几十年的时间。如果继续今天这样打字到2050年，可能很多词汇会因为输入法的关系渐渐消失。维特根斯坦说“语言的界限就是思想的界限”。那这样，整个人类的思想就会自己创造出来的echo chamber给限制住。


作为实验手段，我从淘宝买了人民日报1940年到2017年的数据集，去分析里面汉字的频率。可以看到很多90年代的低频字和2010年的低频字有不一样的特点。90年代的低频字更多字形简单，而2010年的低频字发音简单。我觉得这是因为输入法从五笔到拼音的转变。我有一个小本子的类似想法，大部分都无疾而终。这些想法有两个共同点：1) 悲天悯人的空想，2) 不是一个小博士生有资源运作的。时间久了，很多想法就淡掉了。


特意翻了字典，查了“神棍”的翻译，发现我理解的“神棍”意思和字典并不一样。字典里说神棍就是胡说的人。Harry Frankfurt 有一篇特别有名的短文叫[On Bullshit](http://www2.csudh.edu/ccauthen/576f12/frankfurt__harry_-_on_bullshit.pdf)。讲的是胡说的人和骗子其实不一样。骗子其实关心真相，但是他想把真相藏起来。而胡说的人并不关心真相是什么，他的目标只是吸引别人的注意力，然后说服别人。我觉得神棍是另外一种人。对于科学家而言，真相不可知。神棍只有一个信仰的真相，然后用信仰的理论去指引自己的行为。神棍和胡说的人区别是，神棍自己是相信的。

>这个理论或者也可以应用在比特币的韭菜上。

我之所以觉得神棍是一个很有意思的人格，是因为Jordan Peterson。Jordan Peterson是一个我很羡慕的神棍，他是多伦多大学的教授。Jordan 和Channel 4女主持人的那场[辩论](https://www.youtube.com/watch?v=aMcjxSThD54) 去年在网络上很火。 女主持人问了很多刁钻和引导性的问题，但是Jordan 一直非常冷静。不管什么问题，他都没有被情绪所带走。他似乎有一个笃信的理论，可以解释这个世界的一切现象，然后他遇到所有问题，都是用这个理论来指导他的回答。虽然他的理论未必对，但是他自己是相信的。我想做jordan这样的神棍。


<!-- 我是一个现实而不愿意钻牛角尖的人。第一个问题并没有卡住我很久, 但我始终找不到第二个问题的答案 -->


#### 2. 工程师

Jason可能觉得我不着四六，一入学就想让我去做ai fairness。jason的网站上现在还介绍我是做“ai/ethics”的。16年的时候，一张平等&正义的meme很火，我一开始想做的想法类似于[Equality of Opportunity in Supervised Learning](https://papers.nips.cc/paper/6374-equality-of-opportunity-in-supervised-learning)。做到一半，Moritz Hardt这篇论文就发出来了。我很喜欢这篇论文，Moritz的文章像庖丁解牛，把“公平”这个混乱的观念变成了一个非常具体的数学描述。我想那个时候的自己即便手更快一点，也写不出这么好的论文。

<img src="/resources/justice-fairness.jpg" width="700px" alt="fallingwater"/>

告别神棍是因为两个契机。一个是当我读越来越多的哲学书以后，发现Equality of Opportunity 原来是一个由来已久的概念。哲学家们很早就开始讨论这些，只是没有跟机器学习结合在一起。另外相比于Moritz论文里的简化，哲学家的描述更加精妙，而且充满禅意。然后我带这个问题去问jason，jason给了我一个大智慧的回答。

我问："为什么nsf不把钱给哲学家和社会学家来解决这些问题，他们在这个问题上比我们走得远多了。" 
jason说：“他们这条路走了几百年了，已经被证明很难解决这个问题。从计算机的角度看这些问题，现在虽然比较浅薄，但是是一条新路。”

这个回答让我开始把研究分成“成年的兔子”和“幼年的老虎”，有些研究花更多的精力，也不会变成老虎。论文发表是按体积 (i.e., contributions)来算的，email++比较惨，是一只幼年的兔子，可能做了user study才能成年。

另外一个契机是[The Information: A History, A Theory, A Flood](https://www.amazon.com/Information-History-Theory-Flood/dp/1400096235/ref=sr_1_1?keywords=information&qid=1562442151&s=gateway&sr=8-1)，书里面有一段关于牛顿的论述很精彩。

> The new discipline of physics could not proceed until Isaac Newton appropriated words that were ancient and vague—force, mass, motion, and even time—and gave them new meanings....
For Aristotelians, motion covered a far-flung family of phenomena: a peach ripening, a stone falling, a child growing, a body decaying. That was too rich. Most varieties of motion had to be tossed out before Newton’s laws could apply and the Scientific Revolution could succeed.

牛顿开拓现代物理的第一步其实是定义几个核心观念，比如质量和移动。在很多哲学家眼里，很多广义的变化都可以叫motion，比如小孩长大，桃子成熟。但是现在的“motion”定义更加狭隘，就是从一个位置“移动”到另外一个位置。一句题外话，我非常好奇100年前，中文开始接受现代物理学改造的时候，“移动”是怎么从“运动”中分离出来。

所有这些都把我引向神棍的另外一面：一个好的观点/研究/产品应该有简洁的文字和明快的思想，晶莹剔透，清楚明确。我更喜欢那些有棱角，不含糊的研究，而不是“这个可以那个也可以”的研究。
<b>因为不清不楚的话，自己没办法证明正确，别人也没办法明确指出错误。</b> 我应该是个工程师，既不是设计师也不是哲学家。15年在uist套瓷hiroshi ishii的时候，hiroshi问我“喜欢design么？” 我中二地说了句，“不，我喜欢engineering”。虽然这成了一个非常失败的套瓷，但或者是幸运的。


总之，一方面发现自己想不过那些哲学家，另外一方面觉得自己还是想做解决准确问题而不是创造模糊问题的人，我花了差不多3年才明白自己想走的路。


#### 3. 高立意，低视角

过去一年，我对很多事情发生了改观，比如灌水。我一开始觉得学术圈Publish or perish 的culture是一种toxic的文化。但现在，我觉得灌水是人类系统性科研的一部分，就像小孩子读书要从死记硬背开始([Bloom’s Taxonomy](https://cft.vanderbilt.edu/guides-sub-pages/blooms-taxonomy/))，作家写书靠勤奋而不是灵感([On writing well](https://www.amazon.com/Writing-Well-Classic-Guide-Nonfiction/dp/0060891548))。研究里面偶尔有大跃进，但大部分时候是“积硅步”。当你从更大的视角去看这一切，只要是向前走，一步或者十步其实没那么大区别。

<!-- <img src="/resources/blooms-taxonomy.jpg" width="700px" alt="fallingwater"/> -->


> The key thing about all the world's big problems is that they have to be dealt with collectively. If we don't get collectively smarter, we're doomed. - Douglas Engelbart

这是关于collective wisdom很有名的一句话，但我第一次读这句话的时候却感觉很震撼。我有一种不切实际的理想，觉得人们互相合作应该是1+1>2。因为多人合作有各种思想碰撞的火花。而这句话的期望值要低很多，他陈述了两个观点: 
- 1+1 > 1; 
- 1+1 < 1+1+1 < 1+1+1+1 < 1+...+1.

二年级时，我在纠结我的长期研究方向。那段时间，Jason让我去读了很多白宫的技术报告。这些报告教了我两件事，政府里有很多聪明人对科技有很深的理解，学术圈其实被政府牵着鼻子走。国家意志和国家机器对于科技的追求从来不是来自于个人的兴趣，而是满足整个社会的需要。可能只有在某个微观的瞬间，自己的兴趣和国家的宏观意志对齐在了一起。


<img src="/resources/donkey-carrot.jpeg" width="400px" alt="fallingwater"/>

新闻媒体里有一个很有意思的说法，叫高立意低视角。高立意指的是那些高大上的国家意志议题，高考公平，人民养老，农村生活，诸如此类。低视角说的是那些市民新闻里鸡毛蒜皮的小事，如1818黄金眼。某市民去理发店办了会员卡，不让退款。市民新闻有意思的点是每一个新闻最后都有一堆action items，然后记者会跟踪执行，一直到这件事落实。因为那些事情鸡毛蒜皮，以至于每个人都有共情。而那些高立意的题目因为牵涉太大，更多只是告诉大家有这样的问题存在，却无法去解决这样的问题。


但有一类新闻节目是高立意低视角的: 在鸡毛蒜皮里折射一个大议题。很多时候，这些鸡毛小事最后成了撬动大议题的杠杆。最近让我很感兴趣的新闻助老电梯。国内旧小区里很多老的6层楼房并没有电梯，但是住户年龄增大，国家开始鼓励商业化建造助老电梯。而电梯的建造对于各层楼的住户的利益都不一样, 于是有了各种邻里争吵。这里面有很多有意思的收费方法，比equal opportunity那篇论文更加精彩。


研究最重要的定义是新的, 只要是新的，那就是在向前走。至于有多新，或者有多实用，那只是向前走多少步的区别。今天我对研究的看法和我[17年的时候](http://blog.haojianj.in/posts/me-and-my-research), 发生了一些变化。那个时候，我很同意paul graham对于novelty和goodness的讨论：相比于真实应用，研究是一件很消极的事情。

>  Design doesn't have to be new, but it has to be good. Research doesn't have to be good, but it has to be new. I think these two paths converge at the top: the best design surpasses its predecessors by using new ideas, and the best research solves problems that are not only new, but actually worth solving. - [Design and Research
 by Paul graham](http://www.paulgraham.com/desres.html)


现在，我觉得好的科学研究要借势。首先它要非常具体，这样可以和bullshit区分开，其次它要联系到更大的议题。最后这个具体的问题，是撬动这个大议题很重要的杠杆。过去三年，我对于技术实现的水平未必比读博前更厉害，但我比以前更会画饼了。我攒了很多想做的想法，每一个有着各自的立场(moral ground)。科技的发展，或者随着我有更多的资源，很多本来不可能的想法，渐渐变得可能。去追求这些想法，才是我想要的研究风格。


#### 结尾

本来是想写一个短短的note的，写完读了几遍，让我想起了曹操[让县自明本志令](https://baike.baidu.com/item/%E8%BF%B0%E5%BF%97%E4%BB%A4/4768619?fromtitle=%E8%AE%A9%E5%8E%BF%E8%87%AA%E6%98%8E%E6%9C%AC%E5%BF%97%E4%BB%A4&fromid=890268)的感觉 -- 真把自己当回事。不过趁现在写下来，好过以后忘却。




<!-- 交掉mobicom camera ready的浮生半日闲来写这篇小随笔，写着写着，发现写成了读书笔记。有一本书叫[Made to Stick: Why Some Ideas Survive and Others Die](https://www.amazon.com/Made-Stick-Ideas-Survive-Others/dp/1400064287)， -->

<!-- 
有点像Frank Lloyd Wright设计fallingwater时，压低了窗口处天花板的高度，为了促使住户看向窗外的景色。

<img src="/resources/fallingwater_ceiling.jpg" width="700px" alt="fallingwater"/>
 <i>Fallingwater 是一座建筑史上特别有名的住宅, 建立在匹兹堡附近的一处瀑布旁边。Frank Lloyd Wright 在设计这座住宅时，提倡了一种不同的建筑理念：住宅要完全融入自然之中。每个房间靠近窗口处的天花板都会拉低，强迫房间里的人看向窗外的自然环境。</i> 
 
 


每一个问题都要顺着纹理去切开。


今天各种媒体和直播飞速发展，有很多人在媒体上讨论。这里面我最讨厌的应该是“奇葩说”。




再到最近读Stu Card的[The PhD Thesis Deconstructed](http://hci.stanford.edu/~cagatay/StuCard-WinPrizesGloryPhD.pdf)，讲从混乱到有序是科学研究的本质。
> Think of a PhD professional, her desk surrounded by a little potential energy well of lower entropy relative to the universe, the air cooler, even brisk. Her job is to reduce entropy for others as well by inventing methods, algorithms, and theories usable by them to create order out of chaos. 



这两年我特别讨厌那些把比喻应用在论证里面。
读James Gleick这本书的时候，让我感觉到很庆幸自己是一个工程师而不是哲学家。我不需要去纠结那些飘渺的问题，我可以去直接解决那些已经确定的问题。




作为一个工程师的好处是我不需要去纠结那些虚无的问题，


思考那些悖论不能带来

Reducing entropy 是一件很重要的事。

好的想法应该有简洁的文字和明快的思想。科学的进步伴随的是降低复杂度。


是把一个复杂的问题重新解析，


虽然未必能成功，我还是有“make a difference”的野望，不想从混沌里来到混沌离去。好的科学工作或者产品应该是把一个复杂的问题重新解析，用更简单的方法去四两拨千斤。

薛兆丰的经济学通识里面有一段话



 
 -->