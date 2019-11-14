# sorting-of-changhenge

班级：计181 
姓名：李佳润
学号：2018310740

一、实验题目
  利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能函数，并运行。达到如下功能：

1.每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
2.允许提供输入参数，统计古诗中某个字或词出现的次数
3.考虑操作中可能出现的异常，在程序中设计异常处理程序

输入：汉皇重色思倾国御宇多年求不得杨家有女初长成养在深闺人未识天生丽质难自弃一朝选在君王侧回眸一笑百媚生六宫粉黛无颜色春寒赐浴华清池温泉水滑洗凝脂侍儿扶起娇无力始是新承恩泽时云鬓花颜金步摇芙蓉帐暖度春宵春宵苦短日高起从此君王不早朝承欢侍宴无闲暇春从春游夜专夜后宫佳丽三千人三千宠爱在一身金屋妆成娇侍夜玉楼宴罢醉和春姊妹弟兄皆列士可怜光采生门户遂令天下父母心不重生男重生女骊宫高处入青云仙乐风飘处处闻缓歌慢舞凝丝竹尽日君王看不足渔阳鼙鼓动地来惊破霓裳羽衣曲九重城阙烟尘生千乘万骑西南行<未完，待续>
输出：
汉皇重色思倾国，御宇多年求不得。
杨家有女初长成，养在深闺人未识。
天生丽质难自弃，一朝选在君王侧。
回眸一笑百媚生，六宫粉黛无颜色。
春寒赐浴华清池，温泉水滑洗凝脂。
侍儿扶起娇无力，始是新承恩泽时。
云鬓花颜金步摇，芙蓉帐暖度春宵。
春宵苦短日高起，从此君王不早朝。

二 编写思路
  
  1， 该实验相对来说还是很简单的。我将它分为三个部分即排版、统计与异常处理三部分。
       
	   第一部分：排版
                 通过观察首诗，可以发现，当在第七个汉字后面插入逗号后，在每隔15个汉字再插入一个逗号，这样逗号就插进去了。
              而插入句号则是同理，不过句号第一个位置是15，每隔16位插入一个句号（和逗号数位不同，是因为已经将逗号插入，
              因此插入句号时应该往后移一位）。接下来是换行，换行也是同一样的思路，它是在句号后面进行换行的。
        第二部分：统计
                 该部分应实现输入一个字符，来统计这个字在《长恨歌》出现的次数。因此，我先写了一个输入代码，保证字符串可以
              输入。然后写了一个count函数。在函数中，我用indexOf()来判断n1和n2是否相同。index = n1.indexOf(n2,index))>-1。
              若该条件成立，就用sum 统计出现次数。最后将数值数值返回给count（），再打印出结果。
        第三部分：异常处理
                 对于异常处理，说实话我学的并不好，也就是最基础的try-catch我看不懂怎么用，但是为了满足要求，我只好剑走偏
              锋，用if来进行异常处理。再这个实验中，最容易出现的异常便是空字符。因此我设定了若input的值为空，那么则抛出提
	          示，表示输入不能为空。
 
 2， 流程图
 
         这是流程图
	 
	 
 
              
