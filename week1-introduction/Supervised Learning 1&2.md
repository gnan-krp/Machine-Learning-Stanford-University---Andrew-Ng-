1. Supervised Learning :-
    Supervised learning is the type of machine learning that refers to the algorithm that learns x to y mappings or input to output
    mappings.

                       x      ----------->     y
                     input    ----------->   output
   
    You give the learning algorithm examples that has "right answers" y  for the correct input x.
    By practising this a numerous times the algorithm than learns to have only input x without output y.
    By the input x, the computer than predicts the output y without knowing the correct output. By these
    predictions we can make pecautionary steps for t a better future.
   
-------------------------|----------------------------|---------------------------------------
    input(x)             |    output(y)               |      applications
-------------------------|----------------------------|---------------------------------------
 1.    email             |    spam(0,1)               |      spam filtering
-------------------------|----------------------------|---------------------------------------
 2.    audio             |    textscripts             |      speech recognition
-------------------------|----------------------------|--------------------------------------- 
 3.    English           |    Spanish                 |      machine translation   
-------------------------|----------------------------|--------------------------------------- 
 4.    ad,user info      |    click(0,1)              |      online advertising
-------------------------|----------------------------|--------------------------------------- 
 5.    image,radar info  |    position of other cars  |      self-driving car                             
-------------------------|----------------------------|--------------------------------------- 
 6.    image of phone    |    defect?(0,1)            |      visual inspection
-------------------------|----------------------------|---------------------------------------

There are two types of supervised learning:
    1. Classification Supervised Learning
    2. Regression Supervised Learning

1. Classificaton Supervised Learning:


    |
    |                                                       ex.     size |  diagnosis
    |                                                             -------|-------------  
  1 |                                                                 2  |    0 <------  benign(non-cancerous tumor)
    |                                                                 5  |    1 <------  malignant(cancerous-tumor)
    |                                                                 1  |    0 <------  benign(non-cancerous tumor)
    |                                                                 7  |    1 <------  malignant(cancerous-tumor)
    |                                                                    |
    |
    |
    |
   0| _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
                     tumor size(x)
                    (diameter in cm)


Say you're building a machine learning system so that doctors can have a diagnostic tool to detect breast cancer. This is important
because early detection could potentially save a patient's life. 

Using a patient's medical records your machine learning system tries to figure out if a tumor that is a lump is malignant meaning
cancerous or dangerous. Or if that tumor, that lump is benign, meaning that it's just a lump that isn't cancerous and isn't that
dangerous?

So maybe your dataset has tumors of various sizes. And these tumors are labeled as either benign, which we will designate in this 
example with a 0 or, malignant which we will designate in this example with a 1. 

So let's say we took a tumor size of 2 which a patient is suffering and we will plot this size on the graph, we will tell the system
on the basis of the graph that the tumor size isn't that dangerous. After giving several examples to the system, it will then predict 
the output if the tumor size is dangerous or not dangerous on its own. This type of machine learning is known as classification as
there can only be two outputs 0(not-dangerous) or 1(dangerous).


 2. Regression Supervised Learning:


      |                                                       
      |                                                             
   400|                                                                 
      |                         x    x                                     
   300|                   x  x     x                                              
      |               x x                                                   
   200|          x  x                                                         
      |    x   x
   100|    x  x 
      |  x
     0| _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
        500    1000    1500   2000    2500
              
                 House size
                  in feet2
    
 
In Classification Supervised Learning we gave the algorithm inputs and the output was only between two answers o or 1 i.e. if the tumor 
is benign than the output would be 0 and malignant than out put would be 1. But, what if we want to know the house price in future of 
mine,then the regression supervised learning comes to play.


In this type of ml we give the algorithm several inputs and several outputsat first and when the algorithm starts to learn by itself we ask it to give a closest price at which at a particular size the output would be maximum, the algorithm in this type of ml never says the exact size but gives you the probability percentage that at that particular sied the house price would be at maximum cost.


The method that the algorithm uses is let's say at first it uses the straight line but it is not 100% surity that a straight line will give a more correct output a curve can also give, so it is upto the algorithm which it is will use by analysing the several inputs of the house size.
