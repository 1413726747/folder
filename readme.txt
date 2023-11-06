import turtle
t=turtle.Pen()
t.color('red')
t.fillcolor('red')
t.begin_fill()

t.forward(300)
t.right(90)
t.forward(175)
t.right(90)
t.forward(300)
t.right(90)
t.forward(175)

t.end_fill()

t.color('yellow')
def wu(a,b):
    t.up()
    t.goto(a,b)
    t.down()
    t.begin_fill()
    for i in range(9):
        t.forward(5)
        if i%2==0:
            t.left(180-540/5)
        else:
            t.right(360-540/5*2)
    t.end_fill()    

def wu2(a,b):
    t.up()
    t.goto(a,b)
    t.down()
    t.begin_fill()
    for i in range(9):
        t.forward(10)
        if i%2==0:
            t.left(180-540/5)
        else:
            t.right(360-540/5*2)
    t.end_fill()    

wu2(30,-40)
wu(50,-60)
wu(60,-45)
wu(30,-75)
wu(75,-20)
