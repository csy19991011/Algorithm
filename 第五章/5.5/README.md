#### 问题描述
&emsp;&emsp;给定两个大小为 n 的正整数集合 A 和 B。对于 A 到 B 的一个一一映射 f, 不妨设 $f(a_i) = b_i$ (i = 1,...,n), 则 f 的代价为$\sum_{i=1}^{n} {a_i^{b_i}}$。试设计一个贪心算法, 找出从 A 到 B 的代价最大的一一映射。
#### 问题分析
&emsp;&emsp;**贪心选择性**：不妨设k个正整数的集合A和B都是降序排列，则最优解中必定有$a_1$映射为$b_1$。否则假设$a_1$映射为$b_i$,$a_j$映射为$b_1$,这两个的和为$a_1^{b_i}+a_j^{b_1}$；若两者像互换，则和为$a_1^{b_1}+a_j^{b_i}$，前减后为$(a_j^{b_1}-a_j^{b_i})-(a_1^{b_1}-a_1^{b_i})$从而小于0.</br>
&emsp;&emsp;**优化子结构**: k个正整数的两个集合的最优解中选出最优的一对后，剩下k-1个必然也是最优解。显然</br>
&emsp;&emsp;因此将A与B降序排列后，一一对应即可。
