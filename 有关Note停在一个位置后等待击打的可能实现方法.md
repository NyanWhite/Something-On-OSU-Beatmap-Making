# 绿线

以0.01x作为起始 Higerx作为结尾

0.01-inf之间的距离即为持续时间

其中0x的位置暂时没发现太大影响 但是HigerX的位置以及速度都将会影响所有演出

* 起始时间不影响演出的效果 只影响持续时间

以120bpm为准 底端到顶部的距离为0-1 28通配速

相对的 4x处于0.5的距离 7x已经处于十分接近顶部的位置 7.3-Maxium

1x约在0.1或是0.25的位置

---

# 红线

可适当的添加在演出所需要按下的note之后 以 BaseBPM-infBPM-BaseBPM

间隔距离密一些更好 但不宜小于5ms

另 HigerX的位置添加红线后 红线所对的BPM可调整Note出现位置 这当中可能有些比率 等待探索

1x+800BPM=2x+400BPM=4x+200BPM

纯红线是完全可以实现的



# 应该的思路

设置两个note数据用于读取起始位置以及结束位置

加一个类似于滑块的输入框用于定位减速起始点 a+(b-a)*input%

另一个栏输入时间跳跃间隔时间 也就是用于隐藏之后note的红线的排列密度 如果为0则不使用

手动指定infBPM的倍速



那么如何让Note闪现出来呢

使用高速BPM红线添加在起始点之前几ms即可 然后到达起始点使用BaseBPM