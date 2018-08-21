# Python
1.环境配置  anaconda 和 python 3.6
cmd 分别唤出 python 和 python3（python3.6环境变量 改动为了python3） user\claire\appdata\local\programs\python

2.IDE pycharm  或者直接命令行 用exit()结束

3.先生成.pyc文件 ，import的文件自动生成，非import要命令行里 python -m py_compile a.py   便可生成a.pyc文件 便于保护代码

4.ctrl alt l 自动代码规范

5.ctrl d  复制并换行

6.命令行里 cd 路径  便可切换到某文件路径下工作

7.ctrl / 直接注释该行   等价于 前加#
'''   '''  可多行注释   """   """  也可以

8.ctrl r  替换 

9.变量名只能字母数字下划线，数字不能最前面

10.python3 里输入语句只有content = input（） 得到字符串类型
若要转为原本类型 使用eval()函数 将输入当作代码处理 （对于abc会报错因为没有定义）

11.python2 print 语句
   python3 print（）函数
   
12.python2 输出
#格式化输出
   name="cl"
   age=18
   print"我的名字%s,年龄%d"%(name,age)
   print"我的名字{0},年龄{1}".format(name,age)
#向文件中输出   
   f=open("test.txt","w")
   print>>f,"xxxxxxxx"
#输出不自动换行
   print"1",
   print"2",
   print"3",
#输出各个数据之间分隔符
   print"-".join(["a","b","c"])
   
13.python3 输出
  普通加括号即可
#向文件输出
  print("xxxxxxxxxxxx",file=f)   如果没有创造一个文件来输出
  print("xxxxxxxxxxxx",file=sys.stdout)  直接在控制台输出
#分隔符
  print("a","b","c",sep="*")
#不自动换行
  print("a","b","c",end="")

14.flush  默认为false，但是默认结束带回车，一加回车等于清空缓冲区，如果没有回车，则会在缓冲区中，先执行下面代码
   
15.格式符
mathscore=99
print("%10d" % mathscore)
print("%-10d" % mathscore)   左对齐 10个间隔
print("% d" % mathscore)   加空格与负数对齐  加多少个空格只显示一个

min=5
sec=8
print("%02d:%02d"%(min,sec))   显示 05：08   显示两位数，不够两位拿0补

score=59.9
print("%f"%score)     默认六位小数
print("%.2f"%score)

16. 0b十进制   0o八进制   0x十六进制

17. print("%c"%97)    将数值转换为对应的Unicode码
    score=90
    print("%d%%"%score)   打印％
    %e   将整数浮点数转换为科学记数法
    %d   将整数浮点数转换为十进制
    %o   将整数浮点数转换为八进制
    %x   将整数浮点数转换为十六进制
    不支持%b转换为二进制
    
18.  数字非零即真  字符串非空即真

19.if  xxx：
        xxxxx
   elif xxxxx:
        xxxxx
   else：
        xxxxx

20.print("xxxxx\n"*10)    直接打印10遍












