
![](https://www.python.org/static/img/python-logo.png) 
大蟒蛇

```

运算符
    +加  -减  *乘  /除(得小数)  //整除(得整数)  %余数  =赋值  ==相等  ( )

数据
    数:      0  12  3.14 
    字符串:  '或"括起来的一串字. "和'一样,但必须成对.

练习:
>>> 1+2
3

>>> 'hello '+'张三'
'hello 张三'

>>> '1'+'2'
'12'

>>> 12*3
36

>>> 12/3
4.0

>>> 12//3
4

>>> 7/4
1.75

>>> 7//4
1

>>> 7%3
1

>>> 12%2
0

>>> 11%2
1

>>> 1==2
False


input  输入字符串
print  输出
int    变成整数
eval   去掉引号。例如 "1+2"是字符串，eval("1+2") 是 3

True   真
False  假

not    相反
and    并且
or     或者

变量 ：存储单元(超市的存包柜)

# 输入一个圆的半径(整数),输出它的面积
r=int(input())
s=3.14*r*r
print(s)



#import 导入   random 随机(偶然)   choice 选    ---> 抽奖

# 随机选一件事做
import random
task= random.choice(('吃饭','睡觉','打豆豆'))
print(task)


# 大蟒蛇讲故事
import random  
who= random.choice(("加菲猫","猪八戒","圣诞老人","米老鼠"))
where= random.choice(("救助站","白宫","迪士尼乐园","水帘洞","花果山"))
what= random.choice(("变成一条鼻涕虫爬走了","自燃了","在人行道化成了一坨泥","在众人面前消失了"))
story= ("外边有42度, ", who,"出去遛弯。当走到",where,"时，小伙伴们都惊呆了----" , who , what,
       "。我全程目睹，但没有慌。因为", who, "是一个270斤的胖子，天气又辣么热。:)")
print(*story)



# 三角形面积
a=int(input())
h=int(input())
s=a*h/2
print(s)



# 梯形面积 
a=int(input())
b=int(input())
h=int(input())
s=(a+b)*h/2
print(s)



# 输入三个数，求平方和及平均值
a=int(input())
b=int(input())
c=int(input())
s=a*a+b*b+c*c
y=(a+b+c)/3
print(s)
print(y)



# 输入三边，判断是否直角三角形
a=int(input())
b=int(input())
c=int(input())
if a*a+b*b==c*c or b*b+c*c==a*a or c*c+a*a==b*b:    
    print("是直角三角形")   
else:
    print("不是直角三角形")



# 输入一个整数，判断奇数还是偶数
x=int(input())
if x%2==1:
    print("奇数")
else:
    print("偶数")



# 理财计划 1+2+3+...+n
n=int(input())
s=0
for i in range(1,n+1):
    s=s+i
print(s)



# n的阶乘 1*2*3*...*n
n=int(input())
t=1
for i in range(1,n+1):
    t=t*i
print(t)



# 1~n间偶数的和
n=int(input())
s=0
for i in range(2,n+1,2):  #从2开始,到n,每次增加2
    s=s+i
print(i)



# 平均分>=80晋级
a=int(input())
b=int(input())
if (a+b)/2>=80:
    print("晋级")
else:
    print("淘汰")



# 超市购物金额(整数)>=100打八折，不足100打九折,求实付金额。
x=int(input())
if x>=100:
    print(x*0.8)
else:
    print(x*0.9)



# 分别输入暑假两个月坚持体育锻炼天数，若7月8月锻炼天数均大于等于20天或两个月共锻炼45天（含）以上，
# 输出："运动达人"；否则，输出："加油锻炼"
a=int(input())
b=int(input())
if a>=20 and b>=20 or a+b>=45:
    print("运动达人")
else:
    print("加油锻炼")



# 鸡兔同笼 50头120脚 问几鸡几兔?
for x in range(1,50):
    y=50-x
    if 2*x+4*y==120:
        print("鸡",x,"兔",y)
        break



# 生成二维码qr
import qrcode
qrcode.make('http://www.bing.com').save('bing.png')



```
