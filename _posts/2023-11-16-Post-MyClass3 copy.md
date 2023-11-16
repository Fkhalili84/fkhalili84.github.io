---
layout: posts
title: jungle in fall
---


<body>
<h1 style="text-align: center; font-family: Tahoma;
color: rgb(241, 31, 31);background-color: rgba(116, 243, 91, 0.658);">fall</h1>
<br>
<img src="C:\Users\pentium\Videos\Captures\Python Turtle Graphics 20_08_1402 18_33_32.png" alt="this is a picture of the jungle that I creat with turtle." width="200">
<div style="font-weight: bold; font-size: larger;" dir="rtl">
import random <br>
import time <br>
import turtle <br>
turtle.pensize(600) <br>
turtle.pencolor("olivedrab") <br>
turtle.penup() <br>
turtle.left(90) کشیدن زمین و اسمان با دستورات ساده ترتل بیرون از تابع<br>
turtle.backward(300) <br>
turtle.right(90) <br>
turtle.pendown() <br>
turtle.forward(1000) <br>
turtle.backward(2000) <br>
turtle.left(90) <br>
turtle.pencolor("cadetblue2") <br>
turtle.forward(600) <br>
turtle.right(90) <br>
turtle.forward(2000) <br>
colors1 = ["orange" , "orangered1" , "coral3" , "tan1"] تعریف کردن لیست برای رنگ ها <br>
def leaf1(n): <br>
    turtle.fillcolor(random.choice(colors1)) انتخاب یک رنگ به صورت رندوم<br>
    turtle.begin_fill() شروع به رنگ کردن برگ ها<br>
    for i in range(n): <br>
        turtle.forward(5) <br>
        turtle.right(360/n)تابع رسم برگ <br>
    turtle.end_fill() <br>

def tree(d , a , r): سه متغیر برای درخت در نظر میگیریم<br>
    if d < random.randint(10,11) or a < random.randint(5,6): با دستور روبه رو هیچگاه اندازه شاخه ها زاویه ها از یک اندازه مشخص کمتر نمیشود و در غیر این صورت تابع برمیگردد <br>
        return <br>
    turtle.forward(d) <br>
    turtle.left(a) <br>
    colors = ["coral4" , "salmon4"] <br>
    turtle.pencolor(random.choice(colors)) انتخاب رنگ رندوم برای شاخه ها از بین لیست <br>
    turtle.pensize(r)  اندازه متغیر ها در هر مرحله با ظریب کمتر میشود<br>
    tree(d*(random.random()/2+ 0.5 ) , a*(random.random()/2+ 0.5) , r*0.8) <br>
    turtle.pencolor("orange") <br>
    if d<15: اگر اندازه شاخه ار 15 کمنر باشد برگ رسم میشود<br>
        leaf1(6) این کار از شلوغ شدن درخت ها جلوگیری میکند  <br>
    turtle.right(2*a) <br>
    colors = ["coral4" , "salmon4"] <br>
    turtle.pencolor(random.choice(colors)) <br>
    turtle.pensize(r) <br>
    tree(d*(random.random()/2+ 0.5 ) , a*(random.random()/2+ 0.5) , r*0.8) <br>
    turtle.pencolor(random.choice(colors)) <br>
    tree(d*(random.random()/2+ 0.5 ) , a*(random.random()/2+ 0.5) , r*0.8) <br>
    turtle.left(a) <br>
    turtle.pensize(r) <br>
    turtle.backward(d) <br>
    
turtle.left(90) <br>
turtle.tracer(0) <br>
turtle.penup() <br>
for a in range(10 , 25 , 5): <br>
    for r in range(1 , 5 , 1): <br>
        turtle.pensize(3) <br>
        turtle.penup() در دستور زیر از بین اعداد بازه یک عدد برای جایگاه درخت انتخاب میشود<br>
        turtle.setpos(random.randint(-600 , 600),random.randint(-300 , -200)) <br>
        turtle.pendown() <br>
        tree(80 , 30 , 8) <br>
        turtle.update() <br>
        time.sleep(0.2) <br>

turtle.mainloop() <br>
          
<a href="">

</a>
با دستور ترتل و رندوم در پایتون
</div>

</body>
