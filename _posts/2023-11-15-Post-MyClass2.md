---
layout: posts
title: nice vibe
---


import turtle برای درست کردن درخت باید طبق دستور مقابل ترتل را وارد کنیم 
    def leaf(n):  lتابع های درخت و برگ چپ و راست را تعریف میکنی 
        turtle.fillcolor("orange1") برای رنگ کردن برگ ها از سه دستور در خط های 13 و 14 و18 استفاده میکنیم
        turtle.begin_fill() 
        for i in range(n): 
            turtle.forward(8) 
            turtle.right(360/n) 
        turtle.end_fill() 
    def leaf1(t): 
        turtle.fillcolor("yellow1") 
        turtle.begin_fill() 
        for i in range(t): 
            turtle.forward(8) 
            turtle.right(360/t) 
        turtle.end_fill() 
    def tree(d , r ,n ):سه متغییر تابع درخت به ترتیب برای طول و زاویه بین و ضخامت شاخه ها هستند 
        if d<20 or r<20: 
            return  برای طول و زاویه شاخه ها حد تعیین میکنیم تا در صورت کوچک تر شدن انها تابع ادامه نیابد
        turtle.pencolor("brown") 
        turtle.forward(d) 
        turtle.left(r) 
        turtle.pensize(n) 
        tree(d * 0.75 , r , n*0.75) با جلوتر رفتن طول شاخه ها و ضخامت انها با ظریب کمتر میشود
        turtle.fillcolor("orange1") 
        turtle.begin_fill() 
        turtle.end_fill() 
        turtle.pencolor("yellow1") 
        if d<50: 
            leaf1(6)تا زمانی که شرط بالا برقرار باشد برگ ها بر روی شاخه ها کشیده می شوند 
        turtle.right(2 * r) 
        turtle.pensize(n) 
        tree(d * 0.75 , r , n*0.75) 
        turtle.pencolor("orange1") 
        if d<50: 
            leaf(6) 
        turtle.pencolor("brown") 
        turtle.left(r) 
        turtle.pensize(n) 
        turtle.backward(d) 
    turtle.tracer(0) رسم شکل نهایی بدون نمایش فرایند
    turtle.penup() برداشتن قلم و سپس حرکت کردن
    turtle.right(90) 
    turtle.forward(100) 
    turtle.left(90) 
    turtle.pendown()گذاشتن قلم 
    turtle.bgcolor("lavender") رنگ پس زمینه
    turtle.pensize(10) 
    turtle.left(90) 
    tree(120,40,10) 
    turtle.hideturtle() 
    turtle.mainloop() جلوگیری از بسته شدن پنجره بعد از رسم  



