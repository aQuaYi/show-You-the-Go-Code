# 希尔排序

以下是我对希尔排序的理解。
1. 插入排序的优点是，对于基本有序的序列，可以很快地完成排序。特别地，对于已经排序好的序列进行插入排序，1. 所需时间与序列长度n成正比。
1. 插入排序的缺点是，对于乱序的序列，花费的时间要多得多。特别地，对于逆序的序列进行插入排序，所需时间与1. 序列长度n的平方成正比。
1. 希尔排序是插入排序的改进版本。
1. 希尔排序将大序列分成了h个小序列，小序列中的相邻元素，在大序列中序号相差h。分别对每个小序列进行插入排1. 序。
1. 小序列的插入排序时，小序列相邻元素的交换位置，实际上是大序列中序号相差h的两个元素的交换位置。实现远距1. 离元素交换位置，是希尔排序对插入排序的关键改进。
1. 随着h的减小，每个元素都越来越靠近自己的位置。
1. 当h=1时，最后一个i和j的循环，实际上就是一个大序列的插入排序。这时的大序列已经是基本有序的了。正好可以发挥插入排序的优势。
