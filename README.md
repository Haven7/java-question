# java question
 
# Java经典编程题（持续更新。。。）

不只是java，这些编程题，可以引申到任意一种编程语言内，本例只不过是以java为一种实现。


## 1.指数计算问题

有一对兔子，从出生后第3个月起每个月都生一对兔子，小兔子长到第三个月后每个月又生一对兔子，假如兔子都不死，问每个月的兔子对数为多少？

程序分析： 兔子的规律为数列1,1,2,3,5,8,13,21....

## 2.指定范围包含的素数

判断101-200之间有多少个素数，并输出所有素数。

程序分析：判断素数的方法：用一个数分别去除2到sqrt(这个数)，如果能被整除，则表明此数不是素数，反之是素数。

## 3.水仙花数

打印出所有的"水仙花数"，所谓"水仙花数"是指一个三位数，其各位数字立方和等于该数本身。例如：153是一个"水仙花数"，因为153=1的三次方＋5的三次方＋3的三次方。

程序分析：利用for循环控制100-999个数，每个数分解出个位，十位，百位。

## 4.分解质因数

将一个正整数分解质因数。例如：输入90,打印出90=2*3*3*5。

程序分析：对n进行分解质因数，应先找到一个最小的质数k，然后按下述步骤完成：

```
(1)如果这个质数恰等于n，则说明分解质因数的过程已经结束，打印出即可。
(2)如果n<>k，但n能被k整除，则应打印出k的值，并用n除以k的商,作为新的正整数n,重复执行第一步。
(3)如果n不能被k整除，则用k+1作为k的值,重复执行第一步。
```

## 5.条件运算符使用

利用条件运算符的嵌套来完成此题：学习成绩>=90分的同学用A表示，60-89分之间的用B表示，60分以下的用C表示。

程序分析：(a>b)?a:b这是条件运算符的基本例子。



## 6.公约数和公倍数

输入两个正整数m和n，求其最大公约数和最小公倍数。

程序分析：利用辗除法。

## 7.统计字符串中类型个数

输入一行字符，分别统计出其中英文字母、空格、数字和其它字符的个数。

程序分析：利用while语句,条件为输入的字符不为'\n'.

## 8.求s=a+aa+aaa+aaaa+aa...a的值

求s=a+aa+aaa+aaaa+aa...a的值，其中a是一个数字。例如2+22+222+2222+22222(此时共有5个数相加)，几个数相加有键盘控制。

程序分析：关键是计算出每一项的值。



## 9.指定范围的完数

一个数如果恰好等于它的因子之和，这个数就称为"完数"。例如6=1＋2＋3.编程找出1000以内的所有完数。



## 10.反指数计算

一球从100米高度自由落下，每次落地后反跳回原高度的一半；再落下，求它在 第10次落地时，共经过多少米？第10次反弹多高？



## 11.组合

有1、2、3、4个数字，能组成多少个互不相同且无重复数字的三位数？都是多少？

程序分析：可填在百位、十位、个位的数字都是1、2、3、4。组成所有的排列后再去 掉不满足条件的排列。



## 12.梯度计算

企业发放的奖金根据利润提成。利润(I)低于或等于10万元时，奖金可提10%；利润高于10万元，低于20万元时，低于10万元的部分按10%提成，高于10万元的部分，可可提成7.5%；20万到40万之间时，高于20万元的部分，可提成5%；40万到60万之间时高于40万元的部分，可提成3%；60万到100万之间时，高于60万元的部分，可提成1.5%，高于100万元时，超过100万元的部分按1%提成，从键盘输入当月利润I，求应发放奖金总数？

程序分析：请利用数轴来分界，定位。注意定义时需把奖金定义成长整型。



## 13.求未知数

一个整数，它加上100后是一个完全平方数，再加上168又是一个完全平方数，请问该数是多少？

程序分析：在10万以内判断，先将该数加上100后再开方，再将该数加上268后再开方，如果开方后的结果满足如下条件，即是结果。



## 14.日期计算

输入某年某月某日，判断这一天是这一年的第几天？

程序分析：以3月5日为例，应该先把前两个月的加起来，然后再加上5天即本年的第几天，特殊情况，闰年且输入月份大于3时需考虑多加一天。



## 15.排序

输入三个整数x,y,z，请把这三个数由小到大输出。

程序分析：我们想办法把最小的数放到x上，先将x与y进行比较，如果x>y则将x与y的值进行交换，然后再用x与z进行比较，如果x>z则将x与z的值进行交换，这样能使x最小。



## 16.冒泡排序

输出9*9口诀。

程序分析：分行与列考虑，共9行9列，i控制行，j控制列。



## 17.反推计算

猴子吃桃问题：猴子第一天摘下若干个桃子，当即吃了一半，还不瘾，又多吃了一个 第二天早上又将剩下的桃子吃掉一半，又多吃了一个。以后每天早上都吃了前一天剩下的一半零一个。到第10天早上想再吃时，见只剩下一个桃子了。求第一天共摘了多少。

程序分析：采取逆向思维的方法，从后往前推断。



## 18.数组计算

两个乒乓球队进行比赛，各出三人。甲队为a,b,c三人，乙队为x,y,z三人。已抽签决定比赛名单。有人向队员打听比赛的名单。a说他不和x比，c说他不和x,z比，请编程序找出三队赛手的名单。



## 19.打印出如下图案（菱形）

```
    *
   *** 
 ****** 
******** 
 ****** 
  *** 
   * 
```

程序分析：先把图形分成两部分来看待，前四行一个规律，后三行一个规律，利用双重 for循环，第一层控制行，第二层控制列。



## 20.数列求和

有一分数序列：2/1，3/2，5/3，8/5，13/8，21/13...求出这个数列的前20项之和。

程序分析：请抓住分子与分母的变化规律。



## 21.求1+2!+3!+...+20!的和

程序分析：此程序只是把累加变成了累乘。



## 22.利用递归方法求5!。

程序分析：递归公式：fn=fn_1*4!



## 23.递归计算

有5个人坐在一起，问第五个人多少岁？他说比第4个人大2岁。问第4个人岁数，他说比第3个人大2岁。问第三个人，又说比第2人大两岁。问第2个人，说比第一个人大两岁。最后问第一个人，他说是10岁。请问第五个人多大？

程序分析：利用递归的方法，递归分为回推和递推两个阶段。要想知道第五个人岁数，需知道第四人的岁数，依次类推，推到第一人（10岁），再往回推。



## 24.倒序打印

给一个不多于5位的正整数，要求：一、求它是几位数，二、逆序打印出各位数字。



## 25.回文数

一个5位数，判断它是不是回文数。即12321是回文数，个位与万位相同，十位与千位相同。



## 26.匹配单词

请输入星期几的第一个字母来判断一下是星期几，如果第一个字母一样，则继续 判断第二个字母。

程序分析：用情况语句比较好，如果第一个字母一样，则判断用情况语句或if语句判断第二个字母。



## 27.求100之内的素数



## 28.对10个数进行排序

程序分析：可以利用选择法，即从后9个比较过程中，选择一个最小的与第一个元素交换， 下次类推，即用第二个元素与后8个进行比较，并进行交换。



## 29.求一个3*3矩阵对角线元素之和

程序分析：利用双重for循环控制输入二维数组，再将a[i][i]累加后输出。



## 30.比较排序

有一个已经排好序的数组。现输入一个数，要求按原来的规律将它插入数组中。

程序分析：首先判断此数是否大于最后一个数，然后再考虑插入中间的数的情况，插入后此元素之后的数，依次后移一个位置。



## 31.将一个数组逆序输出。

程序分析：用第一个与最后一个交换。



## 32.取一个整数a从右端开始的4～7位。

程序分析：可以这样考虑：

```
(1)先使a右移4位。
(2)设置一个低4位全为1,其余全为0的数。可用~(~0<<4)
(3)将上面二者进行&运算。
```

## 33.打印出杨辉三角形（要求打印出10行如下图）

程序分析：
 1
 1 1
 1 2 1
 1 3 3 1
 1 4 6 4 1
 1 5 10 10 5 1



## 34.输入3个数a,b,c，按大小顺序输出。

程序分析：利用指针方法。



## 35.选择排序

输入数组，最大的与第一个元素交换，最小的与最后一个元素交换，输出数组。



## 36.交换位置

有n个整数，使其前面各数顺序向后移m个位置，最后m个数变成最前面的m个数



## 37.排序问题

有n个人围成一圈，顺序排号。从第一个人开始报数（从1到3报数），凡报到3的人退出圈子，问最后留下的是原来第几号的那位。



## 38.计算字符串总长度

写一个函数，求一个字符串的长度，在main函数中输入字符串，并输出其长度。



## 39.求和

编写一个函数，输入n为偶数时，调用函数求1/2+1/4+...+1/n,当输入n为奇数时，调用函数1/1+1/3+...+1/n(利用指针函数)



## 40.字符串排序。



## 41.递归

海滩上有一堆桃子，五只猴子来分。第一只猴子把这堆桃子凭据分为五份，多了一个，这只猴子把多的一个扔入海中，拿走了一份。第二只猴子把剩下的桃子又平均分成五份，又多了一个，它同样把多的一个扔入海中，拿走了一份，第三、第四、第五只猴子都是这样做的，问海滩上原来最少有多少个桃子？



## 42.809*??=800*??+9*??+1

其中??代表的两位数,8*??的结果为两位数，9*??的结果为3位数。求??代表的两位数，及809*??后的结果。



## 43.求0—7所能组成的奇数个数。



## 44.一个偶数总能表示为两个素数之和。



## 45.判断一个素数能被几个9整除



## 46.两个字符串连接程序



## 47.打印练习

读取7个数（1—50）的整数值，每读取一个值，程序打印出该值个数的＊。



## 48.加密算法

某个公司采用公用电话传递数据，数据是四位的整数，在传递过程中是加密的，加密规则如下：每位数字都加上5,然后用和除以10的余数代替该数字，再将第一位和第四位交换，第二位和第三位交换。



## 49.计算字符串中子串出现的次数



## 50.求平均数

有五个学生，每个学生有3门课的成绩，从键盘输入以上数据（包括学生号，姓名，三门课成绩），计算出平均成绩，将原有的数据和计算出的平均分数存放在磁盘文件"stud"中。





> 所有内容摘自互联网，非商用，侵删。
