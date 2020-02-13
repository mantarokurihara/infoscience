# this is the journal for computer science

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

*2.13.2020*

1. What did we do?

We added a counter and a bar graph to our dice so it records and shows the amount of times each number appears.

2. What did you learn?

I learned that it's very important to NRY (not repeat yourself) to simplify your code.

3. What question(s) do I have?

A line appeared inside my bargraph, why does that appear?

# code
    #variables
    one_counter=0
    two_counter=0
    three_counter=0
    four_counter=0
    five_counter=0
    six_counter=0

    def setup():
        size(600,600)
        background(255)
    
    def draw():
        #white background
        x=0
        delay(500)
        mouseClicked()
        barGraph()
    
    def barGraph():
        fill(0)
        textSize(20);
        for x in range(6):
            text(x+1,50+50*x,580)
    
    stroke(255,0,0)
    rect(50, 550 - one_counter, 12, one_counter)
    stroke(255,150,0)
    rect(100, 550 - two_counter, 12, two_counter)
    stroke(255,255,0)
    rect(150, 550 - three_counter, 12, three_counter)
    stroke(0,255,0)
    rect(200, 550 - four_counter, 12, four_counter)
    stroke(0,255,255)
    rect(250, 550 - five_counter, 12, five_counter)
    stroke(0,0,255)
    rect(300, 550 - six_counter, 12, six_counter)
    
    def mouseClicked():
        global one_counter, two_counter, three_counter, four_counter, five_counter, six_counter
        background(255)
        stroke(0)
        strokeWeight(10)
        fill(255)
        rect(100,100, 400, 400, 10)
        stroke(255,0,0)
    
    n = random(0,6)
    if 0<=n<1:
        circle(300,300, 50)
        one_counter= one_counter + 1
        print("Number of times one has been rolled:",one_counter)
    if 1<=n<2:
        circle(200,200, 50)
        circle(400,400, 50)
        two_counter= two_counter + 1
        print("Number of times two has been rolled:",two_counter)
    if 2<=n<3:
        circle(200,200, 50)
        circle(300,300, 50)
        circle(400,400, 50)
        three_counter= three_counter + 1
        print("Number of times three has been rolled:",three_counter)
    if 3<=n<4:
        circle(200,200, 50)
        circle(200,400, 50)
        circle(400,200, 50)
        circle(400,400, 50)
        four_counter= four_counter + 1
        print("Number of times four has been rolled:",four_counter)
    if 4<=n<5:
        circle(200,200, 50)
        circle(200,400, 50)
        circle(300,300, 50)
        circle(400,200, 50)
        circle(400,400, 50)
        five_counter= five_counter + 1
        print("Number of times five has been rolled:",five_counter)
    if 5<=n<6:
        circle(200,200, 50)
        circle(200,300, 50)
        circle(200,400, 50)
        circle(400,200, 50)
        circle(400,300, 50)
        circle(400,400, 50)
        six_counter= six_counter + 1
        print("Number of times six has been rolled:",six_counter)
