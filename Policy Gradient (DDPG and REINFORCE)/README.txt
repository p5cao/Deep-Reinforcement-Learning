Here I attach two pdf files. One is generated from latex, and the other is produced by web browser.

The orignial ipython file I also attach here, which I used to train under halfcheetah environment for ddpg.

Additionally, there is a file called source, which contains all the ipython files I used to train all environments respectively.




in the code, actor wants maximize the expection of Q, so we want gradient ascent, which is -gradient descent. therefore the loss function of actor is -expection of Q, we use gradient descent to minimize. 

-Q is -critic.forward(states, actor.forward(states)).mean() where 