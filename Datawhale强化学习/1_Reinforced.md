# 1.过程解析
<img width="473" alt="image" src="https://user-images.githubusercontent.com/40928887/121385145-72da4680-c97b-11eb-80e5-65edf39bebb2.png">

>这个就是agent收到environment给的state，然后产生相应的action返回。此时这个过程中源源不断的获得reward;

*一个智能体agent怎么在一个复杂不确定的环境里面最大化他能够获得的奖励。*
<img width="683" alt="image" src="https://user-images.githubusercontent.com/40928887/121385356-9dc49a80-c97b-11eb-8905-647dac565120.png">

# 2.Sequential Decison-making@Delayed Reward
>我们并没有标签来说明我们的每一步动作到底是正确还是错误，必须要等到游戏结束才能够说明。

<img width="679" alt="image" src="https://user-images.githubusercontent.com/40928887/121385480-b92fa580-c97b-11eb-96f4-b2c270e73e67.png">

**我们只能够不断尝试去发现最有利的工作,agent在获得自己能力的过程中,其实就是通过不断地试错探索trial-and-error exploration**

探索exploration和利用exploitation是强化学习中非常核心的问题。

<img width="642" alt="image" src="https://user-images.githubusercontent.com/40928887/121385779-fe53d780-c97b-11eb-8b38-8661e86ecb7c.png">

探索新行为和利用最好的行为，我们这里要做到一个balance～

## 2.1 我们能够获得的只有一个reward siganl奖励信号
并且这个奖励信号是延迟的,就是说环境在很久以后告诉你之前你采取的行为到底是不是有效的。

>Agent在这个强化学习里面学习的话就会变的非常困难，因为你并没有得到及时反馈。

<img width="678" alt="image" src="https://user-images.githubusercontent.com/40928887/121386077-4410a000-c97c-11eb-9bc0-1f7fcb0eab4d.png">

*可能环境可以告诉你这个行为是错误的，但是没有告诉你正确的是什么，而且可能是两分钟之后告诉我错误，告诉我之前的行为到底行不行，所以这个也是DRL和Supervised Learning不同的地方。*

## 2.2 trial-and-error exploration
<img width="670" alt="image" src="https://user-images.githubusercontent.com/40928887/121386280-715d4e00-c97c-11eb-9fda-30fac3ced88f.png">
试错探索

>监督学习获取的这个算法上线upper bound本质上就是labels人类的表现，这个标注结果决定我们无法超过人类。

>强化学习呢这个就是环境里面自己去探索，所以就是有非常大的潜力，可以获得超越人的能力的这个表现

<img width="685" alt="image" src="https://user-images.githubusercontent.com/40928887/121386481-9e116580-c97c-11eb-986d-3c46562ac413.png">

## 2.3 整个过程
1.你会有一堆观测,这里就是每一个观测都是一个轨迹trajectory, 轨迹就是当前frame以及它采取的策略，就是**状态和动作的一个序列。**
<img width="176" alt="image" src="https://user-images.githubusercontent.com/40928887/121386996-e6c91e80-c97c-11eb-87da-abfdeefabc4d.png">

2.最后结束过后，你会知道你到底有没有把这个球击到对方区域，这个就是eventual reward。我们尽可能最大化这个eventual reward。



1.你会有一堆,这里
1.你会有一堆就是
1.你会有一堆
