# 1.turtle库(import turtle as t)

## 注：一开始的方向是水平向右的

### 1.t.forward()---沿箭头方向走()个像素

### 2.t.backward()---后退

### 3.t.right()---向右转

### 4.t.left()---向左转

### 5.移动画笔位置(三个连用)

```python
import turtle as t
t.penup()
t.goto()
t.pendown()
```

### 6.t.color("","")---前一个颜色是线条颜色，后一个颜色是填充绘制的图形的颜色

```python
import turtle as t
t.color()
t.begin_fill()
...
t.end_fill()
```

### 7.t.pensize()---画笔的宽度

### 8.t.hideturtle()---隐藏箭头

### 9.t.clear()---清除

### 10.t.speed()---画图速度(1是最慢 0是光速)	

### 11.t.circle(redius,extent,steps)---画圆

​	redius(半径):半径有正(负),表示在箭头所指的方向的上(下)方画圆

​	extent(弧度):填入角度

​	steps:做此圆的内接正多边形，多边形的边数为steps

### 12.添加画笔：

```python
import turtle
t1=turtle.Pen()
t2=turtle.Pen()
```

### 13.t.tracer()

1.无轨迹显示，只显示最终画的结果 

```python
import turtle as t
t.tracer(0)  #无轨迹显示
t.circle(50)
t.tracer(1)
```

2.有轨迹显示 

```python
import turtle as t
t.tracer(1)  #有轨迹显示
t.circle(50)
```

### 14.t.setheading()---调整箭头的位置 

```python
import turtle as t
t.setheading(90)  #箭头朝上
```

### 15.t.write("内容",font("字体",大小,“normal”))---在箭头所在的位置填字

### 16.t.onscreenclick()---启动屏幕点击侦测功能

```python
import turtle as t
def p(x,y):
    global k  #用全局变量
    k=1
k=0
t.onscreenclick(p)   #点击后k=1
```

# 2.转义字符

![img](https://img-blog.csdnimg.cn/20200902162943273.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3lhd2VpX2xpdTE2ODg=,size_16,color_FFFFFF,t_70#pic_center)