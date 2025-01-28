from turtle import *

# 设置画布和画笔
screensize(400, 300, "pink")
t = Pen()
t.pensize(3)
t.hideturtle()
t.speed(0)  # 设置最高速度

# 绘制中心圆
t.color("black", "#FFD91C")  # 边框黑色，填充黄色
t.begin_fill()
t.circle(50)
t.end_fill()

# 绘制花瓣的函数
def draw_petal():
    t.color("black", "white")  # 边框黑色，填充白色
    t.begin_fill()
    t.circle(500, 18)  # 画大圆弧
    t.circle(20, 180)  # 画小圆弧
    t.right(8)  # 调整方向
    t.circle(500, 18)  # 画大圆弧
    t.end_fill()

# 绘制花瓣
n = 20  # 花瓣数量
k = 360.0 / n  # 每个花瓣之间的角度
t.penup()
t.goto(0, 50)  # 移动到中心圆的上方
for i in range(n):
    t.setheading(i * k)  # 设置朝向
    t.forward(53)  # 移动到花瓣起点
    t.pendown()
    draw_petal()  # 绘制花瓣
    t.penup()
    t.goto(0, 50)  # 返回中心圆上方

# 结束
exitonclick()
