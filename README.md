# mELM
Morphological Extreme Learning Machine
  
### Follow the instruction:

In the terminal, install _scikit-learn_.
```
pip install scikit-learn
```

# Usage in distinct antiviruses

## Antivirus for IoT _malware_ from ARM architectures

python [melm.py](https://github.com/DejavuForensics/mELM/blob/main/melm.py) -tall [Antivirus_Dataset_IoT_SPARC_mELM_format.csv](https://github.com/DejavuForensics/IoT_ARM/blob/main/Antivirus_Dataset_IoT_ARM_mELM_format.csv) -kfold 10 -ty 1 -virusNorm -nh 500 -af dilation -v

```
Tavares-Silva, S.H.M., Lopes-Lima, S.M., Paranhos-Pinheiro, R. et al.
Antivirus solution to IoT malware detection with authorial next-generation sandbox.
The Journal of Supercomputing 81, 151 (2025).
https://doi.org/10.1007/s11227-024-06506-x
```

## Antivirus for IoT _malware_ from SPARC architectures

python [melm.py](https://github.com/DejavuForensics/mELM/blob/main/melm.py) -tall [Antivirus_Dataset_IoT_SPARC_mELM_format.csv](https://github.com/DejavuForensics/IoT_SPARC/blob/main/Antivirus_Dataset_IoT_SPARC_mELM_format.csv) 
-kfold 10 -virusNorm -ty 1 -nh 500 -af dilation -v

```
Pinheiro Henriques de Araújo, I., Mariano Santiago de Abreu, L., Henrique Mendes Tavares Silva, S. et al.
Antimalware applied to IoT malware detection based on softcore processor endowed with authorial sandbox.
Journal of Computer Virology and Hacking Techniques 20, 729–749 (2024).
https://doi.org/10.1007/s11416-024-00526-0
```

## Antivirus for Citadel _malware_

python [melm.py](https://github.com/DejavuForensics/mELM/blob/main/melm.py) -tall [Antivirus_Dataset_PE32_Citadel_mELM_format.csv](https://github.com/DejavuForensics/Citadel/blob/main/Antivirus_Dataset_PE32_Citadel_mELM_format.csv) 
-kfold 10 -virusNorm -ty 1 -nh 500 -af dilation -v

```
Carlos Henrique Macedo dos Santos, Sidney Marlon Lopes de Lima,
XAI-driven antivirus in pattern identification of citadel malware,
Journal of Computational Science, 82 (2024): 102389.
https://doi.org/10.1016/j.jocs.2024.102389.
```

## Antivirus for Java apps
The database is compressed due to the individual file size delimited by github. Download the compressed file (.zip) to your computer and decompress it before running the extreme neural networks.

python [melm.py](https://github.com/DejavuForensics/mELM/blob/main/melm.py) -tall [Antivirus_Dataset_Jar_mELM_format.csv](https://github.com/DejavuForensics/REJAFADA/blob/master/Antivirus_Dataset_Jar_mELM_format.zip) 
-kfold 10 -virusNorm -ty 1 -nh 500 -af dilation -v

```
Pinheiro, R.P., Lima, S.M.L., Souza, D.M. et al. 
Antivirus applied to JAR malware detection based on runtime behaviors. 
Scientific Reports - Nature Research 12, 1945 (2022). 
https://doi.org/10.1038/s41598-022-05921-5
```

## Antivirus for PHP apps

python [melm.py](https://github.com/DejavuForensics/mELM/blob/main/melm.py) -tall [Antivirus_Dataset_PHP_batch_1_mELM_format](https://github.com/DejavuForensics/PAEMAL/blob/master/Antivirus_Dataset_PHP_batch_1_mELM_format.csv) 
-kfold 10 -virusNorm -ty 1 -nh 500 -af dilation -v

```
Lima, S.M.L., Silva, S.H.M.T., Pinheiro, R.P. et al.
Next-generation antivirus endowed with web-server Sandbox applied to audit fileless attack.
Soft Computing 27, 1471–1491 (2023).
https://doi.org/10.1007/s00500-022-07447-4
```

## Antivirus for JavaScript apps
The database is compressed due to the individual file size delimited by github. Download the compressed file (.zip) to your computer and decompress it before running the extreme neural networks.

python [melm.py](https://github.com/DejavuForensics/mELM/blob/main/melm.py) -tall [Antivirus_Dataset_JavaScript_mELM_format.csv](
https://github.com/DejavuForensics/MARADJS/blob/master/Antivirus_Dataset_JavaScript_mELM_format.zip) 
-kfold 10 -virusNorm -ty 1 -nh 500 -af dilation -v

```
de Lima, S.M.L., Souza, D.M., Pinheiro, R.P. et al. 
Next-generation antivirus for JavaScript malware detection based on dynamic features. 
Knowledge and Information Systems 66, 1337–1370 (2024).
https://doi.org/10.1007/s10115-023-01978-4
```

## Theoretical Background

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

<figure>
  <img src="https://github.com/DejavuForensics/mELM/blob/main/dataset/ELM_1.png" alt="Successful performances of the _kernels_ compatible with the datasets.">
  <figcaption>Figure 1: Successful performances of the _kernels_ compatible with the datasets.</figcaption>
</figure>



<figure>
  <img src="https://github.com/DejavuForensics/mELM/blob/main/dataset/ELM_1.png" alt="Unsuccessful performances of _kernel_ Linear on non-linearly separable datasets.">
  <figcaption>Figure 2: Unsuccessful performances of _kernel_ Linear on non-linearly separable datasets.</figcaption>
</figure>

<figure>
  <img src="https://github.com/DejavuForensics/mELM/blob/main/dataset/ELM_3.png" alt="Successful performances of the mELM Erosion kernel in multiple datasets.">
  <figcaption>Figure 3: Successful performances of the mELM Erosion kernel in multiple datasets.</figcaption>
</figure>

<figure>
  <img src="https://github.com/DejavuForensics/mELM/blob/main/dataset/ELM_4.png" alt="Successful performances of the mELM Dilation kernel in multiple datasets.">
  <figcaption>Figure 4: Successful performances of the mELM Dilation kernel in multiple datasets.</figcaption>
</figure>

## Prediction

When it comes to prediction, the neural network estimates a fractional value. By prediction, we mean a forecast with scientific-methodological rigor. To train the neural network, we show it a series of historical data over time. Example, the neural network examines the daily price of oil for the past few years. The output neuron receives the daily oil price. The input neurons receive the events during that time. Events refer to government decisions, elections, coup attempts, and natural phenomena like droughts.

During training, neurons adjust their connections to prioritize periodic events. 
Seemingly irrelevant daily events can affect the daily oil price.
A person would not usually connect a small event to changes in oil prices. The neural network helps people link past events to current oil prices.
Neural networks are helpful in predicting and preventing natural disasters. Neural networks can predict when a flood will happen, giving advanced warning. In synthesis, neural networks play a fundamental role in building smart city metamodels. Smart cities use electronic sensors to gather data and reduce the effects of natural disasters. 

The evaluation of pattern recognition is different from prediction. In the context of pattern recognition, the main metric is accuracy. Neural networks perform better when closer to 100 percent in specific application. In the prediction scenario, the crucial metric is the root mean square error. The closer this is to 0, the better the performance of the neural network. The model aims to predict well by minimizing the gap between expected and actual outcomes.

## K-fold
Cross-validation is a statistical technique. Researchers use it to assess the performance of a machine learning model. It divides the data set into parts, or ‘folds’. You can train and test the model many times on different data subsets. The aim is to ensure that the model generalises well to new and unseen data. The k-fold method is a type of cross-validation. In it, the data set is randomly split into k equal subsets (or folds). The k-fold involves the following steps:

- **Data division**: the data set is divided into k approximately equal parts.

- **Training and testing**: for each of the k folds, the model is trained using k-1 folds and tested on the remaining fold.

- **Repeating the process**: this process is repeated k times, each time with a different fold acting as the test set.

- **Average and standard deviation of results**: performance metrics are calculated for each of the k runs. For each run, we calculate the average and standard deviation. We then average these metrics. This gives the model's final performance.

## Follow the instructions:

### Parameters of the Extreme Learning Machine:

-    -tr: learning repository reversed to the training phase.
-    -ts: learning repository reversed to the testing phase.
-    -tall: learning repository, this includes the training and testing phase.
-    -kfold: refers to the use of the _k-fold_ method, which must be set to a non-null natural value. As discussed in the previous chapter, _k-fold_ trains the neural network in _k_ runs. In each run, we divide the data set. We use all samples in alternating phases for training and testing.
-    -virusNorm: This config is useful for working with morphological _kernels_. They perform operations based on comparisons and set unions and intersections. For the morphological model to work, synapses between input and hidden neurons must match the sample interval. virusNorm is a normalization technique. It uses malware samples from the VirusShare database as a reference.
[https://virusshare.com](https://virusshare.com).
-    -sep: the delimiter of the statistical learning repository is a regular expression pattern. By default, a space is the delimiter in the _TrainingData_File_ and _TestingData_File_ files. It is a semicolon (;) for the _AllData_File_ file.
-    -ty:
        -    1: classification (pattern recognition). 
        -    0: regression (prediction: prediction with scientific-methodological rigor).
-    -nh: number of neurons in the hidden layer.
-    -af: activation function.
        - Kernel Linear (default): linear
        - Kernel mELM Dilation: dilation
        - Kernel mELM Erosion: erosion
        - Kernel Fuzzy-Erosion: fuzzy-erosion or fuzzy_erosion
        - Kernel Fuzzy-Dilation: fuzzy-dilation ou fuzzy\_dilation
        - Kernel Bitwise-Erosion: bitwise-erosion ou bitwise\_erosion
        - Kernel Bitwise-Dilation: bitwise-dilation ou bitwise\_dilation
        - Kernel Sigmoid: sig or sigmoid
        - Kernel Sine: sin or sine
        - Kernel Hard Limit: hardlim
        - Kernel Triangular Basis Transfer Function: tribas
        - Kernel Radial Basis Function: radbas
-    -sd: random number generator seed.
-    -v: verbose output.

### Didactic repository for pattern recognition:

-	It is not within the scope of this package to create the database. A third party has already created the learning repository. This structure follows the methodology of the ELM inventors.
-	In the path **dataset/classification/diabetes_train**, you can see the structure of the repository as shown in Fig. 5. 
    - **First column**: 1; the sample (row) belongs to the class. 0; the sample (row) belongs to the counter-class.
    - **Other columns**: input attributes (neurons) referring to features of the target application. In this diabetes_train, there are 8 input neurons. For example, in the first sample (row), the first neuron has a value of 0.11764700.
- At the end of learning (training), the ELM neural network will be capable of generalization. The ELM will classify the unseen sample as either class (1.0) or counter-class (0.0). An unseen sample refers to a sample not presented during training.
-    In the terminal, use the extreme neural network in didactic repository. Here's an example:
   
python [melm.py](https://github.com/DejavuForensics/mELM/blob/main/melm.py) -tr [diabetes_train](https://github.com/DejavuForensics/mELM/blob/main/dataset/classification/diabetes_train) -ts [diabetes_test](https://github.com/DejavuForensics/mELM/blob/main/dataset/classification/diabetes_test)  -ty 1 -virusNorm -nh 100 -af dilation -v

<figure>
  <img src="https://github.com/DejavuForensics/mELM/blob/main/dataset/ELM_5.png" alt="Structure of a pattern recognition repository for the use of ELM as a classifier.">
  <figcaption>Figure 5: Structure of a pattern recognition repository for the use of ELM as a classifier.</figcaption>
</figure>

### Authorial repository for pattern recognition:

-	In the path **dataset/classification/Antivirus_Dataset_PE32_Citadel_mELM_format.csv**, you can see the structure of the repository as shown in Fig. 6.
- **First column**: popular name of the file that makes up the dataset.
- **Second column**: corresponds to the output attribute of the repository. 1; the sample (line) belongs to the class (_citadel_ _malware_). 0; the sample (line) belongs to the counter-class.
- **More columns**: the input neurons in the database used correspond to the repertoire of instructions, the calls to the operating system (_syscall_) and the dependencies of the suspect application. In the dataset in figure 6, there are 430 input neurons. For example, in the first sample, the first neuron corresponds to the instruction 'aaa' and has a value of 0.
- In the terminal, use the extreme neural network in professional repository. Here's an example:
  
python [melm.py](https://github.com/DejavuForensics/mELM/blob/main/melm.py) -tall [Antivirus_Dataset_PE32_Citadel_mELM_format.csv](https://github.com/DejavuForensics/Citadel/blob/main/Antivirus_Dataset_PE32_Citadel_mELM_format.csv) 
-kfold 10 -ty 1 -virusNorm -nh 500 -af dilation -v

<figure>
  <img src="https://github.com/DejavuForensics/mELM/blob/main/dataset/ELM_6.png" alt="Structure of a repository for pattern recognition of _malware_ with a view to using ELM as a classifier.">
  <figcaption>Figure 6: Structure of a repository for pattern recognition of _malware_ with a view to using ELM as a classifier.</figcaption>
</figure>

### Didactic repository for prediction:

-	It is not within the scope of this package to create the database. A third party has already created the learning repository. This structure follows the methodology of the ELM inventors.
-	In the path **dataset/dataset/regression/sinc_train**, you can see the structure of the repository as shown in Fig. 7. 
    - **First column**: floating value to be estimated.
    - **Second column**: input attribute (neuron). This is a didactic and hypothetical database. A real application could have hundreds of input neurons.
- At the end of learning (training), the ELM neural network will be capable of prediction. The ELM will estimate a floating value from a given input neuron. 
-    The "mELM" package has a didactic dataset for prediction. It follows the methodology of the creators of ELM. However the authorial structure allows people to experiment with databases in real-world situations. These follow the structure shown in Figure \ref{fig:8_71}. In prediction problems, the second column must be a floating value. We only use classes in pattern recognition.
-    You can use databases from [Kaggle](https://www.kaggle.com/) or [UCI](https://archive.ics.uci.edu/datasets). Search for repositories on their websites that specialize in predicting and analyzing time series.
-    In the terminal, use the extreme neural network in didactic repository. Here's an example:

python [melm.py](https://github.com/DejavuForensics/mELM/blob/main/melm.py) -tr [sinc_train](https://github.com/DejavuForensics/mELM/blob/main/dataset/regression/sinc_train) -ts [sinc_test](https://github.com/DejavuForensics/mELM/blob/main/dataset/regression/sinc_test) 
-ty 0 -nh 100 -af dilation -v

<figure>
  <img src="https://github.com/DejavuForensics/mELM/blob/main/dataset/ELM_7.png" alt="Structure of a repository for prediction using ELM as a regressor.">
  <figcaption>Figure 7: Structure of a repository for prediction using ELM as a regressor.</figcaption>
</figure>




