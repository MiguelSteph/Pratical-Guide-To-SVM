# A Practical Guide to SVM with TensorFlow
**This code belongs to the ["A Practical Guide to SVM"](https://migsena.com/a-practical-guide-to-svm-part-1-data-exploration/) blog post.**

We implement the pratical procedure proposed by **Chih-Wei Hsu**, **Chih-Chung Chang**, and **Chih-Jen Lin** in their paper [**A Practical Guide to Support Vector Classification**](https://www.csie.ntu.edu.tw/~cjlin/papers/guide/guide.pdf).

**Support Vector Machine** (SVM) is a popular technique in machine learning for classification and regression. It is highly preferred by many as it produces significant accuracy with less computation power. The paper proposed a simple procedure to obtain reasonable results from SVM.


## Dataset
In this work, we use the Astroparticle dataset which is a binary classification dataset. A preprocessed version of the dataset can be downloaded [**here**](https://www.csie.ntu.edu.tw/~cjlin/papers/guide/data/). The dataset contains **4 features** and is splitted into training set and test set. The training set contains **3089** rows and the the test set contains **4000** rows. 

## Model performance
The following tableau summarize the performance of the models we have implemented with the proposed procedure: 

|                     | Accuracy | Precision |  Recall  | F1-Score |
| ------------------- | -------- | --------- | -------- | -------- |  
| Simple SVM          | 0.95875  | 0.95875   | 0.95875  | 0.95874  |
| SVM with RBF kernel | 0.96725  | 0.96726   | 0.96725  | 0.96724  |

We see that we have some improvement in all the metric with the RBF kernel.

## Useful Links
- http://danielhnyk.cz/creating-your-own-estimator-scikit-learn/
- https://scikit-learn.org/dev/developers/contributing.html#rolling-your-own-estimator
- https://github.com/nfmcclure/tensorflow_cookbook/tree/master/04_Support_Vector_Machines/04_Working_with_Kernels