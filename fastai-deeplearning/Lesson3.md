1.  What letters are often used to signify the independent and dependent variables?

    > independent variables: X  
    > dependent variables: y

2.  What's the difference between the crop, pad, and squish resize approaches? When might you choose one over the others?
    > as the input data need to be in the same size, while the pictures downloaded online are all in different shapes, we need to re-size them. Crop would be a beter one as it is automatically object-centered(enabled in fastai), and keep the shape of objects.
3.  What is data augmentat ion? Why is it needed?

    > use limited data points differently to reduce overfitting. E.g. cropping one img randomly as different imgs, or flipping the img, chaging the lighting the img.

4.  What is the difference between item_tfms and batch_tfms?

5.  What is a confusion matrix?

    > it is a way to display the model prediction result, including true positive, true negative, false positive and fals negative.

6.  What does export save?

    > the learner (learnt and able to predict)

7.  What is it called when we use a model for getting predictions, instead of training?
    > inference
8.  What are IPython widgets?

    > widgets that allow coders to build interactive prototypes on jupyter notebook.

9.  When might you want to use CPU for deployment? When might GPU be better?

    > when large quantities of parallel programming & running is desired, GPU is better (why large quantities? as gpu only works when there are large amount of work to parallelize).  
    > when only proceed one task at a time, CPU is more co-efficient.

10. What are the downsides of deploying your app to a server, instead of to a client (or edge) device such as a phone or PC?

11. What are three examples of problems that could occur when rolling out a bear warning system in practice?

12. What is "out-of-domain data"?

13. What is "domain shift"?

    > implement the model pre-trained in one domain to another domain. it is one form of transfer learning.

14. What are the three steps in the deployment process?

    > manual process, limited scope deployment and gradual expansion.

15. How is a grayscale image represented on a computer? How about a color image?

    > a grayscale image is represented by x by x matrix  
    > a color image is represented by 3 by x by x matrix

16. How are the files and folders in the MNIST_SAMPLE dataset structured? Why?

    > each number has a seperate folder, and each number folder has a training folder and a validation folder.
    > imgs stored inside are named by sequence o,1,...,n.png

17. Explain how the "pixel similarity" approach to classifying digits works.

    > take the average of each pixels in each group as the "perfect x", and then predict the class by calculating the clostest "perfect x".

18. What is a list comprehension? Create one now that selects odd numbers from a list and doubles them.

    > it is a convenient way to in python to create list with simple functions wrapped inside.

            [i for i in ls if np.mod(i,2)==1]

19. What is a "rank-3 tensor"?

    > sometime like a "3-D cube"; a tensor that has 3 axises.

20. What is the difference between tensor rank and shape? How do you get the rank from the shape?

    > shape: the length of each axis in the tensor.  
    > rank: the length of a tensor's shape, we can use the code below to get the rank out of a tensor's shape:

    ```
    len(tensor_a.shape)
    ```

21. What are RMSE and L1 norm?

    > RMSE means root of mean squre error, it is L2 norm;  
    > L1 norm means the absolute different between 2 numbers.

22. How can you apply a calculation on thousands of numbers at once, many thousands of times faster than a Python loop?

    > by using broadcasting.

23. Create a 3×3 tensor or array containing the numbers from 1 to 9. Double it. Select the bottom-right four numbers.

    ```
    (tensor(range(1,10)).reshape(3,3)[-2:,-2:])*2
    ```

24. What is broadcasting?

    > a way that tensors can be calculated very fast parallelly. For example, a 1010*28*28 tensor can do mse operation with a 28\*28 tensor by broadcasting.

25. Are metrics generally calculated using the training set, or the validation set? Why?

26. What is SGD?
    > stochastic gradient descent
            w -= gradient(w)*lr
27. Why does SGD use mini-batches?
    What are the seven steps in SGD for machine learning?

28. How do we initialize the weights in a model?

29. What is "loss"?

30. Why can't we always use a high learning rate?
31. What is a "gradient"?

- pytorch tensor
  > it is very similar to numpy array, but better. As it can be computed in GPU.
