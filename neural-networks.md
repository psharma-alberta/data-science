
#### Book: [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/index.html)

#### 1: Using neural nets to recognize handwritten digits

##### Perceptrons

###### Perceptron

takes several binary inputs and produces a single binary output

###### Weights

numbers expressing the importance of the respective inputs to the output

###### Threshold 

determines neuron's output based on whether the weighted sum is less than or greater than it

output is 0 if weighed sum is less than threshold, 1 if weighed sum is greater than threshold

###### Bias

measure of how easy it is to get the perceptron to fire

really big bias == easy for the perceptron to output a 1, bias is very negative == difficult for the perceptron to output a 1


##### Sigmoid neurons

###### Sigmoid neuron

small changes in their weights and bias cause only a small change in their output

input: any values between 0 and 1 (instead of 0s or 1s)

output: σ(w⋅x+b), where σ is called the sigmoid function (instead of 0 or 1)

###### Sigmoid function

defined by σ(z) ≡ 1 / 1 + e^(−z)

σ(z) = 1, when z is large and positive

σ(z) = 0, when z is large and negative

σ(z) = 0.5 z=0, 0.73 z=1, 0.88 z=2, 0.95 z=3, 0.98 z=4

##### The architecture of neural networks

###### Multilayer Perceptrons or MLPs

layed network of sigmoid neurons, not perceptrons

###### Feedforward neural networks

neural networks where the output from one layer is used as input to the next layer

###### Recurrent neural networks

these have neurons which fire for some limited duration of time, before becoming quiescent


##### A simple network to classify handwritten digits

##### Learning with gradient descent

- our goal in training a neural network is to find weights and biases which minimize the quadratic cost function




#### Videos

[Neural networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi) - 3Blue1Brown
