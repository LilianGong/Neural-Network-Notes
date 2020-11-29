1.  Why can't we use accuracy as a loss function?

    > as the gradient is very small, for many times it won't change the final accuracy. Therefore, we cannot use accuracy as a loss function as it cannot tell whether a model is improved or not for each weight update.

2.  Draw the sigmoid function. What is special about its shape?

    > usage of sigmoid function: take big numbers to 0 and 1.

        def sigmoid(x): return 1/(1+torch.exp(-x))

3.  What is the difference between a loss function and a metric?

    > the purpose of a loss function is measuring if the model is improved during training; the purpose of a metric is measuring the "goodness" of the model prediction result.

4.  What is the function to calculate new weights using a learning rate?

What does the DataLoader class do?
Write pseudocode showing the basic steps taken in each epoch for SGD.
Create a function that, if passed two arguments [1,2,3,4] and 'abcd', returns [(1, 'a'), (2, 'b'), (3, 'c'), (4, 'd')]. What is special about that output data structure?
What does view do in PyTorch?
What are the "bias" parameters in a neural network? Why do we need them?
What does the @ operator do in Python?
What does the backward method do?
Why do we have to zero the gradients?
What information do we have to pass to Learner?
Show Python or pseudocode for the basic steps of a training loop.
What is "ReLU"? Draw a plot of it for values from -2 to +2.
What is an "activation function"?
What's the difference between F.relu and nn.ReLU?
The universal approximation theorem shows that any function can be approximated as closely as needed using just one nonlinearity. So why do we normally use more?
Why do we first resize to a large size on the CPU, and then to a smaller size on the GPU?
If you are not familiar with regular expressions, find a regular expression tutorial, and some problem sets, and complete them. Have a look on the book's website for suggestions.
What are the two ways in which data is most commonly provided, for most deep learning datasets?
Look up the documentation for L and try using a few of the new methods is that it adds.
Look up the documentation for the Python pathlib module and try using a few methods of the Path class.
Give two examples of ways that image transformations can degrade the quality of the data.
What method does fastai provide to view the data in a DataLoaders?
What method does fastai provide to help you debug a DataBlock?
Should you hold off on training a model until you have thoroughly cleaned your data?
What are the two pieces that are combined into cross-entropy loss in PyTorch?
What are the two properties of activations that softmax ensures? Why is this important?
When might you want your activations to not have these two properties?
Calculate the exp and softmax columns of <<bear_softmax>> yourself (i.e., in a spreadsheet, with a calculator, or in a notebook).
