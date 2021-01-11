
# DAVIAN Lab. Deep Learning Winter Study (2021)

- **Writer:** Min-Jung Kim

## Information

- **Title:** (cs229) Lecture 4 : Perceptron. Exponential Family. Generalized Linear Models.
- **Link:** http://cs229.stanford.edu/notes2020fall/notes2020fall/cs229-notes1.pdf   
http://cs229.stanford.edu/livenotes2020spring/cs229-livenotes-lecture4.pdf
- **Keywords:** Perceptron, Exponential Family, Generalized Linear Model, Softmax Regression (Multi-class classification)

## Perceptron
Perceptron is somewhat similar to sigmoid function but different.   
It is hard version of sigmoid function.   

- **Logistic Regression with Sigmoid function**   
<img src="Images/sigmoid_function.png"></img>    
   
- **Perceptron**   
<img src="Images/perceptron.png"></img>    
   
- **Geometrical Interpretation of Perceptron theta update.**   
<img src="Images/perceptron_update.png"></img>    

> Perceptron is not something that's widely used in practice.   
> We study it mostly for historical reasons.   
> It is not used because it does not have a probabilistic interpretation of what 's happening.      
> Also it could never classify xor   

## Exponential Family
It is class of probability distributions, whos PDF can be written in the form   
   
- <img src="http://latex.codecogs.com/gif.latex?\dpi{110}&space;p(y;\eta)=b(y)exp[\eta^{T}T(y)-a(\eta)]\textbf{}" title="http://latex.codecogs.com/gif.latex?\dpi{110} p(y;\eta)=b(y)exp[\eta^{T}T(y)-a(\eta)]\textbf{}" /> => integrates to 1
      
> y : data (output)   
> <img src="http://latex.codecogs.com/gif.latex?\dpi{110}&space;\eta" title="http://latex.codecogs.com/gif.latex?\dpi{110} \eta" /> : natural parameter (parameter of distribution)   
> b(y) : base measure   
> T(y) : sufficient statistic. In this lecture, T(y) = y    
> <img src="http://latex.codecogs.com/gif.latex?\dpi{110}&space;a(\eta)" title="http://latex.codecogs.com/gif.latex?\dpi{110} a(\eta)" /> : log partition, normalizing constant

### Ex1 : Bernoulli Distribution
**Bernoulli Distribution**
<img src="http://latex.codecogs.com/gif.latex?\dpi{110}&space;p(y;\phi)=\phi^y(1-\phi)^{1-y}" title="http://latex.codecogs.com/gif.latex?\dpi{110} p(y;\phi)=\phi^y(1-\phi)^{1-y}" />   
<img src="http://latex.codecogs.com/gif.latex?\dpi{110}&space;\phi" title="http://latex.codecogs.com/gif.latex?\dpi{110} \phi" /> : probability of event   

**proof**   


### Ex2 : Gaussian Distribution (with fixed variance)
