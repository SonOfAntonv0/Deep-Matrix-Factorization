# Matrix Completion by Deep Matrix Factorization

A PyTorch implementation of Deep Matrix Factorization (<a href=https://github.com/jicongfan/Matrix-completion-by-deep-matrix-factorization>Link</a> to original code which is implemeted by using MATLAB.)<br>

<h2> Matrix Completion </h2><br>
Matrix completion is the task of filling in the missing entries of a partially observed matrix. We consider the example 
of the movie ratings matrix that was a part of the Netflix problem in this work. Given a ratings matrix 
in which each entry (i,j) represents the rating of movie j by user i. We know myriad techniques of imputing 
missing values by the column's mean, mode or median. Such approaches fail to consider any interaction between the features.
To address that caveat, Matrix Factorization is leveraged for Matrix Completion.<br>

![](https://user-images.githubusercontent.com/30777433/108379003-81192100-722b-11eb-8c78-7c2a79e573df.png)
Linear Matrix Factorization

<br>
<h2> Deep Matrix Factorization</h2><br>
Given a matrix X, Matrix Factorization involves approximating X as the outer product of two matrices, U and V.
Matrix factorization is a linear method, meaning that if there are complicated non-linear interactions going on 
in the dataset, a simple dot product may not be able to handle it well. Hence, we leverage NNs to learn
a non-linear function, say f, of U and V that best approximates X. <br>

![](https://user-images.githubusercontent.com/30777433/108375915-6d1ff000-7228-11eb-9d0d-92277c562f9e.png)
Deep Matrix Factorization

<br>
References

[1] J. Fan and J. Cheng, “Matrix completion by deep matrix factorization,” Neural Networks, vol. 98, pp. 34 – 41, 2018. 

