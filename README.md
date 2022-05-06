### Neural Networks
- setup.

2D self-driving car



 we're creating a feed-forward neural network.
 are a special NN that does not form a self loop?
comparable to a single layer perceptron.

starts of as single layer but as each children car comes out, there's hidden layers being added, sadly my code doesn't work for 
the hidden layer I couldn't fix it.

since it's perceptron
it's MSE - mean squared error.
and there's other advanced features on this package, also it has in-built learning optimization
Error = `1−∑i(ei−ai)2`

this particular model takes in fuzzy set input
tried binary but it was too inaccurate

pygame is a drawing package that's enables vectors graphics and things to be drawn.

had to prepare assets.

also `pypi` is kinda wonky to use.

+ created `requirements.txt` for reference.

the gens are cool, but the cars keep lagging or crashing, faster learning = tweaking the road width variables.


 is an evolutionary algorithm that creates artificial neural networks

 ANNs



 Forward Neural Network is commonly seen in its simplest form as a **single layer perceptron**.

 can only classify linearly separable cases with a binary target

 activation function is `tanh`


`road.py` - road generation
road was generated using a common random object generating algorithm
is actually a collection of points, which are connected, in order to make the car detection efficient.

so technically the car calculates closest point, and then calculates the distance.

 `world.py` - general helper function for car coordinates
 `vect2d` - helper function with vector calculations
 `node.py` - helps drawing functions for `NNdraw.py`

 we calculate something called `fitness`
 which is used to positively / negatively re-enforce the car.
 this is the target they have to reach.

 and it keeps automatically updating.

 the weights -> A,B,C,D,E,F,G,H + speed

 ![](/documentation/car-weights.png)  


 ![](/documentation/parent-child-topology.png)  

 ![](/documentation/screenshot-entire.png)  

**EASY MODE**
 lowering maximum speed, lesser tighter turns

 there's currently a problem in the neural network not using the brake at all, i'm not sure why that's a thing.



 at the end of the run when all cars are dead, 
 -> allowed to generate children which will then run after on.

children will def carry over the characteristics

they keep adding more hidden layer networks over every iteration, so the visible performance is seen.

it's sorta like a winner takes all, we're also letting them compete with each other.
but not using **maxnet**, but a more primitive like the top 2 performers are chosen and then those are iteratively 
used.



There's also a bit of an error where the car exits the given road.

after every epoch the performance keeps getting better and better



### interesting observations 
is that the car finds creative ways to break the game and keep following.
so let's say once the car broke the fence, and then the further children will learn that they will crash in that exact same spot
and keep repeating it, because it gives the best score.

it's performance should be comparable to a single layer perceptron.

A multilayer perceptron (MLP) is a fully connected class of feedforward artificial neural network