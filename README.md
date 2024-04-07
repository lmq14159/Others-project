# School-Project
<h2>一、画图</h2>

1.变形vk图：画个跟这个一样的图，就是按这些不同分组的数据画

![2d461dee6820d9c78921dfe69c01ba9](https://github.com/lmq14159/Others-project/assets/82321147/a847f319-95db-4303-a824-fca46936540e)

2.kmd：用给的数据文件（1.csv）的数据画，D列数据为X轴，Z列数据为Y轴

<img width="357" alt="f57689c792cf6427ae4f2220e17e506" src="https://github.com/lmq14159/Others-project/assets/82321147/dfaf4e83-5522-4ae4-a1b5-d5c5b6087530">

3.百分比图：用给定的百分比的文件里的数据画，这个有五个柱

![8568cdde0968a3ae474e4268e9e663c](https://github.com/lmq14159/Others-project/assets/82321147/3e996159-945d-4a63-96f3-c1d1bddfbca0)+

![7b6ca7d10879ce5dabff5d1d53e03ac](https://github.com/lmq14159/Others-project/assets/82321147/ae717aa3-b555-4b10-9103-84416809943d)

4.dbc-c图：用给定的数据文件（1.csv）的相应数据画图

![image](https://github.com/lmq14159/Others-project/assets/82321147/1ba28827-ee94-4938-a6c2-715f3444989a)



======================================================================================================================================================

<h2>二、非靶向质谱版(统计版)</h2>
在现在的基础上修改：</br>
1.分子量需要通过iupac文件换算后替换原来的分子量；</br>
2.最后的展示文件（count.csv）需要加上各自的强度（原始数据的strength这一列）；</br>
3.最后需要将相同的分子质量差的结果的个数由高到低排序后进行输出；</br>
4.需要能同时处理多个文件。



======================================================================================================================================================



<h2>三、网络分析</h2>
使用igraph等网络分析工具创建网络并计算参数。</br>
使用节点和边文件创建网络，然后计算：网络的度（Degree，与某个分子有联系的分子数量）、 度中心性（Degree centrality， 体现分子核心性（重要性）， 该值越大说明该分子越重要，属于较活跃的分子，反之，该分子较不活跃）、 亲密中心性（Closeness centrality，体现分子影响力，该值越大说明该分子在整个样品中的辐射能力约强，即，除了与近端分子有直接联系，还可能与远端分子存在间接联系）、间接中心性（Betweenness centrality，体现分子作为中间过渡性分子的重要性，数值越大说明该分子在整个网络中具有较强的连接作用）、 特征向量中心性（Eigenvector centrality，体现分子与邻近核心分子的关系，数值较大说明该分子与很多核心分子存在关系，该分子属于核心分子的联系或过渡分子）。 </br>
参考资料：</br>
https://python.igraph.org/en/stable/generation.html</br>
https://cloud.tencent.com/developer/article/1625275</br>
https://zhuanlan.zhihu.com/p/426397948



======================================================================================================================================================


<h2>四、业绩统计</h2>
表中前6个sheet第一列是已经支付的订单号码，后面3个sheet（所有订单）第一列是所有的订单号，在所有订单中查收未支付的订单。输出未支付订单的所有信息





======================================================================================================================================================


<h2>五、分类</h2>
1.将文件1.csv中的数据按照O、NO和SO进行分类，例：O这一列下数值为2且N和S列的数值为0就分类为O2，N列为1同时O为8且S为0分类为N1O8，S为1同时O列为2且N列为0分类为O2S1，其他（O、S、N列数值均不为0）分为others类，结果写到文件的最后一列。</br>
2.计算不同类别的不同dbe（数据文件的第24列）的强度（数据的第二列）和，每一个类别都有不同大小的dbe（计算dbe为1-20的数据），例：N1O3类别下的dbe3的强度为：该类别下所有dbe等于3的强度相加，其他以此类推，每个类别都有20个dbe强度和。</br>
3.能够进行批量文件的处理


======================================================================================================================================================


<h2>六、关键路径</h2>
使用igraph等网络分析工具创建名为关键路径的分子网络，原始数据文件node.csv中的source列为起始节点，target列为终点节点，使用fr或其他布局方法，实现与效果图中类似的效果

======================================================================================================================================================


<h2>七、点阵框图</h2>
数据文件中前面是4个框的边界线的范围，后面是在几个框组合上画的点图的数据![图例](https://github.com/lmq14159/School-Projects/assets/82321147/25cad5a7-e219-4682-b3d6-d3852964649b)


======================================================================================================================================================


<h2>八、K-shell算法</h2>
先将1.csv中的数据建立为网络，然后使用K-shell算法识别其中的关键节点。
K-shell算法思想和具体过程：
![image](https://github.com/lmq14159/School-Projects/assets/82321147/3bdbf850-e528-4061-804f-a7a1d4988b8c)
![image](https://github.com/lmq14159/School-Projects/assets/82321147/0d2b3800-4adb-4604-858b-8e231c5650da)
参考资料：
http://jst.tsinghuajournals.com/article/2022/4313/1650946547417-1198530195.htm#outline_anchor_1



