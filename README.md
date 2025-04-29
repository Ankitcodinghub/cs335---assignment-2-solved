# cs335---assignment-2-solved
**TO GET THIS SOLUTION VISIT:** [CS335 – Assignment 2 Solved](https://www.ankitcodinghub.com/product/cs335-assignment-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;111160&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS335 - Assignment 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Instructions

• This assignment should be completed individually.

• Do not look at solutions to this assignment or related ones on the Internet.

• The files related to the assignment are present in lab2-rollno.zip folder. Extract it and upload it on moodle in the same .zip format after completion and after replacing the string “rollno” with your actual roll number. For example, if you roll number is 00405036, then single zip folder that you will upload will be named “lab2-00405036.zip”. Also collate all the CS337 based theory solutions into ONE pdf file named answers.pdf. Include answers.pdf inside the zip folder mentioned above and submit the zip folder.

• Answers to all subjective questions need to be placed in single pdf answers.pdf including all plots and figures and uploaded.

• Only add/modify code between TODO and END TODO unless specified otherwise • The code for all the questions should be written in provided ipython notebook only. Don’t modify the name/directory structure of the provided .zip file.

• Please make sure that your code runs in python 3.x. You shuld not import any new python libraries.

• Code should be written in the provided assignment 2.ipynb file only.

1 Perceptron

A Perceptron keeps a weight vector wy corresponding to each class y. Given a feature vector f, we score each class y with

score(f,y) = Xfiwyi

i

where i iterates over the dimensions in the data. Then we choose the class with the highest score as the predicted label for data instance f.

f1 f2 y

0 0 0

0 1 0

1 0 0

1 1 1

Table 1: AND Dataset

Learning the weights of the Perceptron

In the basic multi-class Perceptron, we scan the entire training data, one instance at a time. When we come to an instance (f,y), we find the label with the highest score: y0 = argmax score(f,y00),

y00

while breaking ties arbitrarily. We compare y0 to the true label y. If y0 = y, we have correctly classified the instance, and we do nothing. Otherwise, we have wrongly predicted y0 instead of the true label y. This means that wy has scored f lower, and/or wy0 has scored f higher, than what would have been ideally desirable. To avert this error in the future, we update these two weight vectors accordingly: wy = wy + f and wy0 = wy0 − f

1.1 CS 337: Theory

1. An alternative to the 1-vs-rest perceptron defined above is to have a 1-vs-1 perceptron, one for each pair of classes. Compare this proposed 1-vs-1 approach to the previously described 1-vs-rest approach for multi-class classification. Outline and briefly justify the advantages and disadvantages of each. (1 mark)

2. Assume a data point (f,y) which got misclassified as y0. Show that the above update rule increases score(f,y) and decreases score(f,y0). (1 mark)

4. For a dataset, assume that the upper bound on number of iterations required for convergence of perceptron is M. If we change the perceptron update rules as follows:

wy = wy + 0.5f wy0 = wy0 − 0.5f

Comment on the upper bound on number of iterations under the modified algorithm. (0.5 mark)

5. For AND dataset given by the AND function as mentioned in the Table 1, Compute the upper bound on the number of iterations required by the Perceptron algorithm. (1 mark)

1.2 CS 335: Lab

Implement 1-vs-rest perceptron algorithm described above. Complete the function perceptron() in the notebook. (2.5 mark)

Data Description

For this assignment, we assume a ground truth function y = f(x) = 1 − 3x − 2×2 + 2.5×3. However, to exploit the feature selection property of LASSO we have added few redundant features to the dataset. You have to learn a lasso model which should be able to detect the redundant features from the dataset.

2 LASSO and ISTA

Lasso regression uses the `1 penalty term and stands for Least Absolute Shrinkage and Selection Operator. It is a widely used tool for achieving sparse solutions to optimization problems. The penalty applied for `1 is equal to the absolute value of the magnitude of the coefficients.

In matric form (using matrix X here instead of Φ as used in the class, LASSO optimizes

In this problem, we will implement the Iterative Soft-Thresholding Algorithm (ISTA) for LASSO.

2.1 CS 337: Theory

1. Prove that the solution to LASSO is the MAP estimate of Linear regression subject to the

Laplacian prior on weights. (1.5 mark)

2. Similar to ridge regression, a lambda value of zero results in the basic OLS equation, however given a suitable lambda value, lasso regression can give more sparse solution as compared to ridge regression. Discuss the reason behind this property of lasso. (1 mark)

3. Does the closed form solution for Lasso exist? If yes, then mention the conditions for which closed form solution will be possible. Give your answer with explanations. (1 mark)

2.2 CS 337: Lab

1. Complete the ista() function in file assignment 2.ipynb. You can reuse the relevant functions you had implemented in Assignment 1. You can modify lr, epochs and λ, if needed.

Add the generated figures in the report. (2.5 mark)

2. Complete the mse multi var(), mse regularized(), split data(), multivar reg closedform() functions. (1 mark)

3. Analyze how LASSO does feature selection using the ista() function. Compare the weights obtained from Lasso and Ridge Regression by creating a single plot. For Ridge, you can use the code from previous assignment. (2 mark)

3 Bias Variance Trade-off

3.1 CS 337: Theory

(a) Increasing the value of λ in lasso regression.

(b) Increasing model complexity by adding more features of high degree.

(c) Reducing dimension by choosing only those subset of features which are of more importance.

3.2 CS 337: Lab
