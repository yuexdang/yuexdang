# yuexdang
python作业

                   #1
a=1
i=input("输入你要的数：")
i=int(i)
for s in range(1,i+1):
    a=a*s

print("i!的答案是:",a)

                 #2
a=1
n=input("输入你要的数：")
n=int(n)
k=0
for s in range(1,n+1):
    a=a*s
    k=a+k

print("n!的答案是:",k)

                  #3
import math
print("给予a,b,c值为5,8,3")
print("解a*x*x+b*x+c=0")
a=5
b=8
c=3
lll=math.sqrt(b**2-4*a*c)
t1=float((-b+lll)/(2*a))
t2=float((-b-lll)/(2*a))
print("方程的解分别是:",t1,t2)

                #4
m=input('输入一个正整数:')
k=m
n=len(m)
x=list(m)
for s in range(1,n):
    for v in range(0,s-1):
        if int(x[s-v])>int(x[s]):
            print(x[s-v],x[s])

                #5
a=input('请输入字符串a:')
b=input('请输入字符串b:')
print('字符串a的长度为',len(a))
x=''.join(reversed(a))
y=b
print('新字符串为:',x+y)
k=b.find(a,0,len(b))
if k!=-1:
    print('a是b的子串')
else:
    print('a不是b的子串')

                         #6
import random

a= random.sample('abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789',1)
b= random.sample('abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789',1)
c= random.sample('abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789',1)
d= random.sample('abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789',1)

k=a+b+c+d
k=list(k)
k=''.join(k)
print(k)
n=input('请输入验证码:')

if n==k:
    print("验证码正确！")
else:
    print('验证码错误！')

	#7
x=input('输入一个字符串:')
x=x.swapcase()
print(x)

                #8
x=input('请给定一个字符串:')
y=len(x)
z=input('请指定要检索的字符:')
print (x.find(z,0,y))

                           #9
import datetime


idc=input("请输入您的身份证号码:")


oo=datetime.date.today()
oo=int(oo.year)

str=idc
pp= str[6:10]
zz= str[10:12]
ll= str[12:14]
uu=pp+"年"+zz+"月"+ll+"日"
nn=int(oo)-int(pp)

qq=int( str[16])
if qq%2==0:
    kk="女"
else:
    kk="男"

ass="*****************************************************************************"
print(ass)
print("    身份统计:")
print("    性别:"+kk)
print("    生日:"+uu)
print("    年龄:",nn)
print(ass)

                #10
l=input('请输入一个字符串:')
l=list(l)
x=[]
for s in l:
    z=ord(s)
    x.append(z)

print(x)

                  #11
y=int(input("请输入一个数:"))
k=0
for e in range(0,y,2):
    k=k+e

print('偶数合为:',k)

                #12
def k(s):
    abc_num = 0
    digit_num = 0
    other_num = 0
    for i in s:
        if i.isalpha():
            abc_num += 1
        elif i.isdigit():
            digit_num += 1
        else:
            other_num += 1
    return('中英文字符有',abc_num,'个','数字有',digit_num,'个','其他字符有',other_num,'个')
m=input('请输入字符串:')
m = k(m)
print(m)

                    #13
pp=input('输入一个字符串:')

str=pp
x= str[-8:]

if x=='back-end':
    print('Yes')
else:
    print('No')


                         #14
a=input("输入第一个数:")
b=input("输入第二个数:")
c=input("输入第三个数:")

p=[]

p.append(a)
p.append(b)
p.append(c)

print("三个数中最大的数是:",max


                         #15
year=int(input('请输入年份:'))

#表示对判断是否是年份有疑惑，下列是考虑了公元前情况的程序


if year<=0:
    print("输入格式错误，不存在负数年份")

else:

    if year%100!=0:
        x=year%4
        if x==0:
            print(year,'是闰年')
        else:
            print(year,'不是闰年')

    else:
        if year%400==0:
            print(year,'是闰年')
        else:
            print(year,'不是闰年')

		#16
b=[]
for x in range(100,1000):
    o=x
    x=str(x)
    x=list(x)
    k=int(x[0])**3+int(x[1])**3+int(x[2])**3
    x=o
    if k==x:
        b.append(o)

print(b)

                #17
i=input('请输入一个数值加入列表Is中:')
x=[]
x.append(int(i))
print('tips:输入"exit"终止元素添加')
while type(i)!=int():
    i=input('请输入一个数值加入列表中:')
    if i=='exit':
        print('列表元素添加完毕')
        break
    else:
        x.append(int(i))
        
q=len(x)
u=[]
for c in range(0,q):
    t=x.pop(c)
    l=1
    for v in range(0,q-1):
        y=x[v]
        l=y*l
    u.append(l)
    x.insert(c,t)

print(u)

		
	#18
x=int(input('请输入一个正整数:'))
l=0
#自动认定从零到X不包括X
for o in range(0,x):
    if o%3==0 or o%5==0:
        p=o
        l=p+l

print('最终结果是',l)

	#19
i=input('请输入一个数值加入列表中:')
x=[]
x.append(int(i))
print('tips:输入"exit"终止元素添加')
while type(i)!=int():
    i=input('请输入一个数值加入列表中:')
    if i=='exit':
        print('列表元素添加完毕')
        break
    else:
        x.append(int(i))

k=int(input('请输入一个K值:'))
x.sort()
x.reverse()
print(x)
print('K对应的的数值为:',x[k])

                #20
tou=int(input('请输入头的数量:'))
zu=int(input('请输入足的数量:'))

ji=2*tou-zu/2
tu=zu/2-tou

print('共有',ji,'只鸡')
print('共有',tu,'只兔')

                #21
import turtle
turtle.setup(800,800,800,800)


#脸
turtle.penup()
turtle.goto(-210,0)
turtle.seth(-90)
turtle.pendown()
turtle.pencolor('orange')
turtle.pensize(4)
turtle.begin_fill()
turtle.circle(210,360)
turtle.fillcolor('yellow')
turtle.end_fill()
turtle.pencolor('black')

#左眼
turtle.penup()
turtle.pensize(4)
turtle.goto(-180,90)
turtle.pendown()
turtle.seth(40)
turtle.begin_fill()
turtle.circle(-120,80)
turtle.penup()
turtle.goto(-180,90)
turtle.pendown()
turtle.seth(-130)
turtle.circle(15,110)
turtle.seth(40)
turtle.circle(-106,83)
turtle.seth(30)
turtle.circle(18,105)
turtle.fillcolor('white')
turtle.end_fill()
turtle.pensize(4)
turtle.penup()
turtle.goto(-150,95)
turtle.pendown()
turtle.begin_fill()
turtle.circle(10,360)
turtle.fillcolor('black')
turtle.end_fill()

#右眼
turtle.penup()
turtle.goto(20,90)
turtle.pendown()
turtle.seth(40)
turtle.begin_fill()
turtle.circle(-120,80)
turtle.penup()
turtle.goto(20,90)
turtle.pendown()
turtle.seth(-130)
turtle.circle(15,110)
turtle.seth(40)
turtle.circle(-106,83)
turtle.seth(30)
turtle.circle(18,105)
turtle.fillcolor('white')
turtle.end_fill()
turtle.pensize(4)
turtle.penup()
turtle.goto(50,95)
turtle.pendown()
turtle.begin_fill()
turtle.circle(10,360)
turtle.fillcolor('black')
turtle.end_fill()

#嘴
turtle.pensize(4)
turtle.penup()
turtle.goto(-180,30)
turtle.pendown()
turtle.seth(-92)
turtle.circle(180,180)

turtle.hideturtle()
turtle.done()


                #22
import time
import calendar
y = int(time.strftime("%Y",time.localtime()))
m = int(time.strftime("%m",time.localtime()))
d = int(time.strftime("%d",time.localtime()))
print('当前时间为:',y,'年',m,'月',d,'日')

uuu = [31,29,31,30,31,30,31,31,30,31,30,31]
if calendar.isleap(y) == False:
    uuu[1]=28

xxx=0
for i in range(0,m-1):
    xxx=xxx+uuu[i]

print("今天为今年的第",xxx+d,"天")

                           #23
print("转换方式有℃转化为℉，℉转化为℃")
print('要℃转换请输入1，℉转换请输入2')
L=input("请选择转换方式:")

if L=='1':
    X= float(input("请输入摄氏温度:"))
    K=X*33.8
    print("华氏温度为:",K)
elif L=='2':
    X= float(input("请输入华氏温度:"))
    K=X/33.8
    print('摄氏温度为:',K)


                #24
for i in range(1,10):
    for j in range(1,i+1) :
        print(j,'x',i,'=',i*j)


                         #25
import random
X=random.randint(0,100)

print("欢迎玩猜数字游戏 \n系统将随机生成一个0～100的数值，你有7次猜数机会")
print('游戏开始')


a=0
while a<=6:
    Y=int(input("请猜这个数的数值:"))
    if Y>X:
        print('你猜的数值偏大了')
        a=a+1
        
    elif Y<X:
        print('你猜的数值偏小了')
        a=a+1
        
    elif Y==X:
        print('你猜对了')
        break
while a>6:
    print('你的机会已用尽，答案是:',X)
    break

#26不存在

                #27
o=1
n=int(input('请输入一个n值:'))
a=0
b=1
c=0
x=[]
while o<=n:
    x.append(b)
    b=int(b)
    c=a
    a=b
    b=c+b
    o=o+1

print('斐波那契数列中第',n,'项的值为',x[-1])

			#28
m=int(input('输入正整数m:'))
n=int(input('输入正整数n:'))
ooo=[]
ppp=[]
if m>=n:
    print('格式错误,请使m<n')
else:
    for k in range(m,n):
        o=len(str(k))
        l=list(str(k))
        for r in range(0,o):
            for i in range(0,r):
                if l[r]>l[i]:
                    if k >= 2:
                        if k % 2 !=0:
                            for ii in range(2,k):
                                if k % ii == 0:
                                    ppp.append(k)
                                else:
                                    ooo.append(k)
                                
                                if k % ii ==0:
                                    ooo.remove(k)

ooo=list(set(ooo))
ooo.sort()
print('最终结果是',ooo)

		#29
h=float(input('请输入身高:'))
w=float(input('请输入体重:'))
class B():
    def __init__(self,height,weight):
        self.height=height
        self.weight=weight
        
   
    def BMI(self):
          return self.weight/(self.height**2)


b= B(h,w)
print(b.BMI)

		#30	
class Doge():

    def bark():
        print('this hanpi dog start pa~~~')
    
    def creep():
        print('mou~~~')

Doge.bark()
Doge.creep()	
