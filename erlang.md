shell:strings(false) 
["⢡","✔","✓","⥬","⟣","✒","⟞","⟙","⢣","⟢","⥫","⟚","⢪","⢢"]
当成汉字了

Erlang shell 接入控制台
windows   werl       -detached 
方法1. JCL模式 Ctrl + G
erl -setcookie abc -name node_1@127.0.0.1 
设置相同的cookie 
erl -setcookie abc -name node_2@127.0.0.2 
Eshell V8.1  (abort with ^G)
(node_2@127.0.0.1)1> node().
'node_2@127.0.0.1'
(node_2@127.0.0.1)2> 
User switch command
 --> j
   1* {shell,start,[init]}
 --> r 'node_1@127.0.0.1' 
 --> j
   1  {shell,start,[init]}
   2* {'node_1@127.0.0.1',shell,start,[]}
 --> c 2
Eshell V8.1  (abort with ^G)
(node_1@127.0.0.1)1> 

方法2. -remsh
erl -setcookie abc -name node_3@127.0.0.3 -remsh node_1@127.0.0.1 
注意. 禁止 q(). 
可以使用 Ctrl + c 两次 来终止
Ctrl + G  Q

ps aux | grep beam  
检查进程

方法3. https://www.iteye.com/blog/mryufeng-362394

io:format() 详解
___
##  Record & Map 
> Erlang程序设计第二版第五章
  ### 何时使用 Record 记录
  - 当你可以用一些预先确定且数量固定的原子来表示数据时;
  - **当记录里的元组数量和元素名称不会随时间而改变时**;
  - 当存储空间是个问题时,典型的案例是你有一大堆元组,并且每个元组都有相同的结构.
  ### 何时使用 Map 映射组
  - 当键不能预先知道时用来表示键-值数据结构;
  - 当存在大量不同的键时用来表示数据;
  - 当**方便使用**很重要而**效率无关紧要**时作为万能的数据结构使用 ;
  - 用作 __"自解释型"__ 的数据结构,也就是说,用户容易从键名猜出值的含义;
  - 用来表示键-值解析树,例如XML或配置文件;
  - 用JSON来和其他编程语言通信.
