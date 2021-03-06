
# Assignment 3 -- Interactive Vis

## 

---

## 可视化主题：权力的游戏1-7季

数据来源：[剧集数据](https://www.kaggle.com/dasbootstrapping/game-of-thrones-episode-data 'data').

可视化结果：[Vis on Game of thrones](https://kenzoyan.github.io/vis-on-game-of-thrones/ 'Vis on Game of thrones'). 

## 动态交互

1. 坐标轴的移动以及放大缩小
2. 鼠标移动到点上浮现点具体信息
3. 选中某一点，能够得到该集所在季的在两幅图中的相关信息
4. 按住Shift键，可以选取多个点，在图表中进行对比比较.
5. 在图表中间添加了control bar,方便直接选择感兴趣的项目进行比较

**浮现具体信息**

![tooltip](/photos/1.jpg)

**选择数据单独观察**

![select](/photos/2.jpg)

**选中多组数据进行对比**

![tooltip](/photos/3.jpg)


## 数据解读

整个图表分为两个部分，左右两边分别是散点图和折线图。

### 散点图：

主要表现的是**观众人数**，**贵族死亡人数**，**剧集第几季**的之间的关系,颜色和形状都是用来区分属于第几季的，虽然可能会觉得有点重复了，用两个属性表示一个维度，但是我自己觉得两个都有的时候会更容易看出来对比，更加容易区别。
**颜色**:

![](/photos/4.jpg)

**颜色+形状**:

![](/photos/5.jpg)

### 折线图

主要表现的是**每一季中剧集的评分变化趋势**的关系，因为是可交互的，所以可以只选择某一季的评分，在这一季里面进行对比。也可以自己选择多个季的数据，在季和季之间进行评分变化的比较。

### 图片结论

1. 总体每一季的观众人数都是在一直增长的。但是四五六季增长的幅度很小，第七季的增长幅度是最大的。
2. 和前几季相比，从第七季开始主要角色的死亡人数就有了比较大的下降。
3. 第五季的评分最不稳定，集与集之间的变化很大。
4. 评分都是总体处于高低之间的循环往复。
5. 重要角色死亡人数多的剧集评分很可好极高或者极低（相对整体），猜测可能是:
>死亡人数多剧集精彩，人们倾向于高打分

>自己喜欢的角色死亡，对剧集打低分


### 花费时间：6 Hours

Altair是一个很方便使用的基于Vega实现的python可视化包

#### 之前构思的草图，基本实现的构思
![draft](/photos/6.png)
