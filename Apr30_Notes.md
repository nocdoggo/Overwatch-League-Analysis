1. 用Dino Football

   1. With pm.Model() as model:

   这个里面的home_theta中的home是不是可以去掉，而且应该如何去除，设定成0？

   2. 如果需要用attack和defense

   如果需要使用这个football model，是不是应该将Team换成hero？然后我们应该有选择性的挑选数据

   而且作为Team，有attack和defense，我们需要考虑的就比较多，不是很practical。

2. **用tennis model [重新看一下上课的视频，看看Dino到底搞了个什么大新闻]**

   1. **Player_skills 到底是啥**
   2. **到底用了哪些variables来确立模型**
   3. **skills？跟我们   stat_name, stat_amount有什么关系**
   4. **那就真的成了hero/队伍天梯图？那这么说，我们2020年数据生成一张天梯图，然后根据2021测试数据生成天梯图，需要similar**
   5. 然后再看获胜的队伍是不是选了更容易胜利的hero，比如说，前10的队伍都用了DVA，但是没用Reinhart，那么可以说DVA是比较容易让我们获胜的hero
   6. 对获胜的队伍的比赛的hero的stats进行分析，然后看某个skill和win_rate之间的关系《------clean_match_merge
   7. ===》你玩DVA的时候，是应该坚持放大招，还是右键按死

   1. 我们能预测哪个队伍会胜利么
   2. 如果胜利了，是不是选了我们预测中的比较强的英雄，而且靠预测中的top技能获胜的
   3. NaN填充成mean

   拿Time_played / match_duration 作为contribution的权重,然后standardize一下，除以标准差

   linear：就这么干了或者**ridge regression** 

   y = Y  = Xβ, 然后beta是有差的range

   做t-test, 看P value是不是小于0.05

   Linear 有一个常数列，如果用sm包，需要开头加一个常数列

   然后看model.summary，constant是常数项，就是误差

   P>|x| < 0.05贡献就很大

   



win



Clasture ? 进行分类，k-means model，不是回归一个数值，而是分成了几大类

3-2 ： A

3-0  ： B

重新做一列出来成为我们的y value，强制做一个映射,

有时间做，没时间摆烂回归

