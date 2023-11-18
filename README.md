# mELM
Morphological Extreme Learning Machine

Neural network is a computational intelligence model employed to solve pattern recognition problems. Neural networks can generalize and recognize new data that wasn't taught during training. In backpropagation strategy, adjusting many parameters is necessary to improve neural network performance. 
The neural network usually gets stuck in local minima. To eliminate these areas, control strategies are added to these networks. The network needs a lot of training time to classify the samples. The latest neural networks are accurate, but training can take many days to complete.

We have developed ELM (Extreme Learning Machine) neural networks. ELMs train and predict data faster than neural networks that use backpropagation and Deep Learning.
Kernels form the basis for learning ELMs networks. The kernels are mathematical functions used as learning method of ELMs neural networks. Kernel-based learning offers the possibility of creating a non-linear mapping of data. You don't need to add more adjustable settings, like the learning rate in neural networks. 

## Pattern Recognition

Kernels are mathematical functions used as a learning method for neural networks. Kernel-based learning allows for a non-linear mapping of data without increasing adjustable parameters. But kernels can have limitations. A linear kernel can't solve a non-linearly separable problem, like a sine distribution. Whereas a sinusoidal kernel may be able to solve a problem as long as it is separable by a sine function. Finding an optimized kernel is a big challenge in artificial neural networks. The kernel helps determine the decision boundary for different classes in an application. 

We introduce mELMs. They are ELMs with hidden layer kernels inspired by image processing operators. We call these operators morphological Erosion and Dilation. We claim that morphological kernels can adapt to any boundary decision. Mathematical morphology studies the shapes of objects in images using mathematical theory. It looks at how sets intersect and join together. Morphological operations detect the shapes of objects in images.  The decision frontier of a neural network can be seen as an n-dimensional image. In this case, n represents the number of extracted features.
The decision frontier of a neural network can be seen as an _n_-dimensional image. In this case, _n_ represents the number of extracted features. mELMs can naturally identify and represent the n-dimensional areas associated with various classes.

Mathematical Morphology is a theory used in digital image processing to process nonlinearly. Various applications like object detection, segmentation, and feature extraction use Mathematical Morphology. Morphology is based on shape transformations that preserve the inclusion relationships of objects. There are two fundamental morphological operations: Erosion and Dilation. Mathematical Morphology is a constructive theory. It builds operations on Erosions and Dilations.

Fig. 1 (b) and Fig. (c) show the result of the Erosion and Dilation operation on the same original image: Fig. 1 (a). In the eroded image, the target object is "withered". In the dilated image, the target object is dilated, as the name suggests. The Dilation kernel expands the region connected to the target class. An analogy is drawn between image processing operations and authorial mELM networks. The Dilation kernel expands the region attached to the target class (e.g. malware). In turn, the Erosion kernel expands the region belonging to the counter-class (e.g. benign).

One major difficulty in artificial neural networks is finding the best kernel for a specific task. ELM neural networks can solve a linearly separable problem using a Linear kernel, as seen in (Fig.). 2 (a). The Sigmoid, RBF, and Sinusoid kernels can solve problems that can be separated by Sigmoid, Radial, and Sinusoidal functions, as shown in Fig. 2 (b), Fig. 2 (c) and Fig. 2 (d), respectively.

A neural network's ability to generalize well can depend on the right choice of kernel. The best kernel may be dependent on the problem to be solved. 
To improve the results, consider studying various kernels for the neural network.
Studying different kernel types is computationally expensive. It requires cross-validation and multiple random starting points. 

To see a counter-example, look at how the Linear kernel is used with the Sigmoid and Sine distributions in Fig. 2 (a) and Fig. 2 (b), respectively. The classification accuracies shown in Fig. 2 (a) and Fig. 2 (b) are 78.71% and 73.00%, respectively. The Linear kernel doesn't clearly show the decision boundaries of Sigmoid and Sinusoid distributions.

Fig. 3 (a), Fig. 3 (b), Fig. 3 (c) and Fig. 3 (d) show the performance of the mELM Erosion kernel on the Linear, Sigmoid, Radial and Sinusoid distributions. The respective accuracies are 100%, 93.07%, 98.18% and 99.50%.  Fig. 4(a), Fig. 4 (b), Fig. 4 (c) and Fig. 4 (d) show the performance of the mELM Dilation kernel on the Linear, Sigmoidal, Radial and Sinusoidal distributions. The respective accuracies of 100%, 95.05%, 98.18% and 99.50%. We can see that the mELMs accurately map various distributions for different problems. It should be noted that the two attributes are normalized to the same lower and upper limit.

The kernels mELMs are successful because they can model any decision boundary. They do not follow conventional geometric surfaces like ellipses and hyperbolas. The mELMs kernels map the decision boundary in _n_-dimensional. The coordinates are based on training samples. _n_ represents the number of extracted features. mELMs can detect and model different classes by using Mathematical Morphology. It detects the shapes of bodies in images.

## Follow the instructions:

-	It is not within the scope of this package to create the database. A third party has already created the learning repository.
-	In the path **dataset/classification/diabetes_train**, you can see the structure of the repository as shown in Fig. 5.
  - **First column**: 1; the sample (row) belongs to the class. 0; the sample (row) belongs to the counter-class.









