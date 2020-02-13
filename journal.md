# This is the journal for Computer Science

*1.30.2020*

1. What did we do?

Today, we looked at the Computational Thinking, which consists of Deconstructing, Pattern Recognition, Abstraction and Algorithm Design.
We applied this process with creating jam sandwiches, and made our own set of instruction that we asked Dr. Pinzon to follow.

2. What did you learn?

I learned that it was surprisingly difficult to give a clear and algorithmic set of instructions for even such a simple task like making a jam sandwich.

3. What question(s) do I have?

How does computational thinking really apply when we start programming?

*2.11.2020*

1. What did we do?

Today, we created our own dice in Processing. We then created a "loaded" or "biased" dice by changing the probability for one of the values, and tried to guess which value was biased for eachother.

2. What did you learn?

I learned how strokes and drawing tools worked in Processing. (e.g strokeWeight, colors) I also learned how to create random numbers and probability codes using (n).

3. What question(s) do I have?

What's the best method when trying to find out the biased value?


def setup():
    size(600,600)
    
def draw():
    # White background
    x=0
    
def mouseClicked():
    background(255)
    stroke(0)
    rect(100,100, 400, 400, 10)
    stroke(255,0,0)
    strokeWeight(10)
    
    n = random(0,3.1)
    if 0<=n<0.6:
        circle(300,300, 50)
    if 0.6<=n<1.1:
        circle(200,200, 50)
        circle(400,400, 50)
    if 1.1<=n<1.6:
        circle(200,200, 50)
        circle(300,300, 50)
        circle(400,400, 50)
    if 1.6<=n<2.1:
        circle(200,200, 50)
        circle(200,400, 50)
        circle(400,200, 50)
        circle(400,400, 50)
    if 2.1<=n<2.6:
        circle(200,200, 50)
        circle(200,400, 50)
        circle(300,300, 50)
        circle(400,200, 50)
        circle(400,400, 50)
    if 2.6<=n<3.1:
        circle(200,200, 50)
        circle(200,300, 50)
        circle(200,400, 50)
        circle(400,200, 50)
        circle(400,300, 50)
        circle(400,400, 50)
