# circle-circle-relation
# python beginner practice

import turtle

t=turtle.Turtle()

t.shape("turtle")

x11=turtle.textinput("","Center coordinates x")     #1st circle' information

x1=int(x11)

y11=turtle.textinput("","Center coordinates y")

y1=int(y11)

r11=turtle.textinput("","radius")

r1=int(r11)

x22=turtle.textinput("","Center coordinates x")    # 2nd circle' information 

x2=int(x22)

y22=turtle.textinput("","Center coordinates y")

y2=int(y22)

r22=turtle.textinput("","radius")   ##1st circle's radius is bigger than 2nd

r2=int(r22)

t.up()

t.goto(x1,y1-r1)

t. down()

t. circle(r1)

t.up()

t.goto(x2,y2-r2)

t.down()

t.circle(r2)


d=((x1-x2)**2+(y1-y2)**2)**0.5

if d>r1+r2 :

    t.write("do not meet.")

elif d==r1+r2:

    t.write("come across at one point.")

elif r1-r2<d<r1+r2 :

    t.write(" meet at two points.")    

elif d==r1-r2:

    t.write("one circle is inside the other while they come across at one point.")
    
elif d<r1-r2 :

    t.write("one circle is inside the other and do not meet.")
