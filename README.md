# 2020_MCM_C
## 问题一
__Analyze the three product data sets provided to identify, describe, and support with mathematical evidence, meaningful quantitative and/or qualitative patterns, relationships, measures, and parameters within and between star ratings, reviews, and helpfulness ratings that will help Sunshine Company succeed in their three new online marketplace product offerings.
分析提供的三个产品数据集，以数学证据来鉴定，描述和支持有意义的定量和/或定性模式，关系，测度和参数。这些将在星级，评论和帮助等级之内和之间进行。__

简而言之，就是数据的处理，把产品数据运用数学语言描述出来。可以自己筛选一定的指标构成因变量与自变量，例如可以把帮助等级构造成因变量，星级和评价构造成自变量。
对于星级评价这种非负计数型变量，最常采用的模型是泊松回归。但泊松分布最大的特点之一就是方差与均值相等，但对于存在过度离势的变量而言，其方差大于均值，与泊松回归的特点相悖，所以泊松回归不能很好地解决。（可以适当说明下）常用的模型之一就是负二项回归。

## 问题二
__A. Identify data measures based on ratings and reviews that are most informative for Sunshine Company to track, once their three products are placed on sale in the online marketplace.
A. 一旦三种产品在在线市场上出售后，就可以根据评级和评论确定阳光公司的最佳测量度。__

即拟合问题。最佳测量度，即自变量，评级和评论，即因变量。可以利用神经网络的方法拟合出自变量与因变量的关系。除了神经网络，还可以采用偏最小二乘回归的方法。结论一定要说清楚，即最佳测量度的具体定义是什么，还有评级和评论是怎么影响它的。

__B. Identify and discuss time-based measures and patterns within each data set that might suggest that a product’s reputation is increasing or decreasing in the online marketplace.
在每个数据集中识别并讨论基于时间的度量和模式，这些度量和模式可能表明产品在在线市场中的声誉在上升或下降。__


__C. Determine combinations of text-based measure(s) and ratings-based measures that best indicate a potentially successful or failing product.
C. 确定最能表明潜在成功或失败产品的基于文本的度量和基于评级的度量的组合。__
此问为预测模型，根据第一问和第二问构建的拟合模型，来求出最坏和最好的情况。即根据因变量的值来反推出自变量的值。可以把最好的情况指标定义为1.最坏的情况时指标定义为0，然后反推出评级和评论的具体结果。

__D. Do specific star ratings incite more reviews? For example, are customers more likely to write some type of review after seeing a series of low star ratings?
D. 特定星级会引起更多评论吗？ 例如，在看到一系列低星级评级之后，客户是否更有可能撰写某种类型的评论？__
此题为因变量的自相关与共轭性问题。在前面的几题中，自变量都是独立的，也是就是互不影响的，此题去掉了这个假设。在第一问回归的基础上，需要考虑因变量是否存在正相关的关系，即星级数值增加，评论会产生何种影响。


__E. Are specific quality descriptors of text-based reviews such as ‘enthusiastic’,‘disappointed’, and others, strongly associated with rating levels?
 E。 诸如“热情”，“失望”之类的描述是否与其他的得分紧密相连？__
 此题为自然语言处理与聚类分析。可以先对词语进行聚类分析。
 
 ##问题三
__Write a one- to two-page letter to the Marketing Director of Sunshine Company summarizing your team’s analysis and results. Include specific justification(s) for the result that your team most confidently recommends to the Marketing Director.
写一两页的信给阳光公司的市场总监，总结您团队的分析和结果。包括针对您的团队最有信心地推荐给市场总监的结果的具体理由。__



