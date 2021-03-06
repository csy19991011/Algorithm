#### 问题描述
&emsp;&emsp;乌龟棋：乌龟棋的棋盘是一行N个格子，每个格子上一个分数（非负整数）。棋盘第1格是唯一的起点，第N格是终点，游戏要求玩家控制一个乌龟棋子从起点出发走到终点。 </br>
&emsp;&emsp;乌龟棋中M张爬行卡片，分成4种不同的类型（M张卡片中不一定包含所有4种类型 的卡片，见样例），每种类型的卡片上分别标有1、2、3、4四个数字之一，表示使用这种卡片后，乌龟棋子将向前爬行相应的格子数。游戏中，玩家每次需要从所有的爬行卡片中选择一张之前没有使用过的爬行卡片，控制乌龟棋子前进相应的格子数，每张卡片用且只能使用一次。游戏中，乌龟棋子自动获得起点格子的分数，并且在后续的爬行中每到达一个格子，就得到该格子相应的分数。玩家最终游戏得分就是乌龟棋子从起点到终点过程中到过的所有格子的分数总和。很明显用不同的爬行卡片使用顺序会使得最终游戏的得分不同。现已知棋盘上每个格子的分数和所有的爬行卡片，求得一种卡片使用顺序使得最终游戏得分最多。</br>
&emsp;&emsp;例：有9个格子上的分数分别为6 10 14 2 8 8 18 5 17，有卡片1 1 1 2 3，则使用爬行卡片顺序为1,1,3,1,2,得到的分数为6+10+14+8+18+17=73。注意，由于起点是1，所以自动获得第1格的分数6。
## 问题分析
&emsp;&emsp;**洛谷P1541**</br>
&emsp;&emsp;只能暴力四维DP,详细讲解可参考洛谷题解。优化子结构显然。