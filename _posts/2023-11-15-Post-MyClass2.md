---
layout: posts
title: nice vibe
---


<body>
<h1 style="text-align: center; font-family: Tahoma;
color: rgb(241, 31, 31);background-color: rgba(116, 243, 91, 0.658);">Tree</h1>
<br>
<img src="C:\Users\pentium\Videos\Captures\Python Turtle Graphics 20_08_1402 18_33_32.png" alt="this is a picture of the tree that I creat with turtle." width="200">
<div style="font-weight: bold; font-size: larger;" dir="rtl">
    import turtle برای درست کردن درخت باید طبق دستور مقابل ترتل را وارد کنیم <br>
    def leaf(n):  lتابع های درخت و برگ چپ و راست را تعریف میکنی <br>
        turtle.fillcolor("orange1") برای رنگ کردن برگ ها از سه دستور در خط های 13 و 14 و18 استفاده میکنیم<br>
        turtle.begin_fill() <br>
        for i in range(n): <br>
            turtle.forward(8) <br>
            turtle.right(360/n) <br>
        turtle.end_fill() <br>
    def leaf1(t): <br>
        turtle.fillcolor("yellow1") <br>
        turtle.begin_fill() <br>
        for i in range(t): <br>
            turtle.forward(8) <br>
            turtle.right(360/t) <br>
        turtle.end_fill() <br>
    def tree(d , r ,n ):سه متغییر تابع درخت به ترتیب برای طول و زاویه بین و ضخامت شاخه ها هستند <br>
        if d<20 or r<20: <br>
            return  برای طول و زاویه شاخه ها حد تعیین میکنیم تا در صورت کوچک تر شدن انها تابع ادامه نیابد<br>
        turtle.pencolor("brown") <br>
        turtle.forward(d) <br>
        turtle.left(r) <br>
        turtle.pensize(n) <br>
        tree(d * 0.75 , r , n*0.75) با جلوتر رفتن طول شاخه ها و ضخامت انها با ظریب کمتر میشود<br>
        turtle.fillcolor("orange1") <br>
        turtle.begin_fill() <br>
        turtle.end_fill() <br>
        turtle.pencolor("yellow1") <br>
        if d<50: <br>
            leaf1(6)تا زمانی که شرط بالا برقرار باشد برگ ها بر روی شاخه ها کشیده می شوند <br>
        turtle.right(2 * r) <br>
        turtle.pensize(n) <br>
        tree(d * 0.75 , r , n*0.75) <br>
        turtle.pencolor("orange1") <br>
        if d<50: <br>
            leaf(6) <br>
        turtle.pencolor("brown") <br>
        turtle.left(r) <br>
        turtle.pensize(n) <br>
        turtle.backward(d) <br>
    turtle.tracer(0) رسم شکل نهایی بدون نمایش فرایند<br>
    turtle.penup() برداشتن قلم و سپس حرکت کردن<br>
    turtle.right(90) <br>
    turtle.forward(100) <br>
    turtle.left(90) <br>
    turtle.pendown()گذاشتن قلم <br>
    turtle.bgcolor("lavender") رنگ پس زمینه<br>
    turtle.pensize(10) <br>
    turtle.left(90) <br>
    tree(120,40,10) <br>
    turtle.hideturtle() <br>
    turtle.mainloop() جلوگیری از بسته شدن پنجره بعد از رسم<br>    
<a href="">

</a>
با دستور ترتل در پایتون
</div>

</body>
