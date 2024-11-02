java c
MATH 524, Fall 2024 
Nonparametric Statistics 
Partial solutions to the first assignment 
1. If X is Bernoulli with parameter p, its cumulative distribution function F is then given by 

Therefore, the random variable Y = F(X) takes the values 1 − p and 1 with probability 1 − p and p, respectively.  It is clearly not uniformly distributed on the interval (0, 1).
2. By the law of total probability, and upon conditioning on the value of X2 , one has 


where the fact that the random variables X1 , X2 , X3   are mutually independent was used. Therefore, upon making the change of variable u = F(x), one finds 


Further note that Pr(X1   < X2 < X3 ) = Pr(R1 < R2 < R3 ). A similar calculation could be done for any other ordering of these three variables or, equivalently, their ranks.  Therefore, the joint distribution of the associated rank vector (R1 , R2 , R3 ) is uniform.
3.     a)  The sum of the ranks of the treated observations is Ws  = 61 and under the null hypothesis, the mean and variance of Wilcoxon’s rank-sum statistic are 9×19/2 = 85.5 and 9×9×19/12 = 128.25, respectively.  With continuity correction, the p-value of the one- sided test is 

where Z denotes a standard Gaussian random variable.  Thus one can reject the null hypothesis at the 5% level and conclude that guinea pigs that were administered vitamin C through orange juice had longer odontoblasts after six weeks. 
b) Using the R command ks. test, one finds that the value of the Kolmogorov–Smirnov statistic is 5/9 = 0.556, and that the cor- responding p-value is 0.06218. The conclusion is then different at level 5%: the null hypothesis fails to be rejected, suggesting that the difference between the two treatments might be due to chance. 
4.    a)  Given that N = m + n = 50, the variance of Ws  under H0  is 
var(Ws ) = (N + 1)mn/12 = 51m(50 − m)/12 . 
This is a quadratic function in m. It is easy to see that its maxi- mum is reached at m = 25.
b)  The number of possible values for the variable is given by

Given that n = 50 − m, one is once again in the presence of a qu代 写MATH 524, Fall 2024 Nonparametric Statistics HW-1R
代做程序编程语言adratic function, the maximum of which occurs at m = 25. 
5.  There are N = 24 observations divided in two groups of size m = 11 and n = 13. Note that there are two ties, so one must use Wilcoxon’s rank-sum test for ties with ℓ = 22 and d10  = d21  = 2.  The ranks are assigned as follows: 

The observed value of Ws*  is 220. Under the null hypothesis that there is no difference between the controls and the treated mushrooms, one has

and


i.e., var(Ws* ) = 297.6144.  As the alternative hypothesis would lead to high ranks for the treated group, the p-value of the one-sided Wilcoxon rank-sum test is given by 


Therefore, there is more than enough evidence to reject the null hy- pothesis. 
6.  There are  (4(8)) = 70 cases in total and a simple enumeration leads to the following null distribution for the Siegel–Tukey statistic An :


7.  Assuming (as one does here) that there are no ties in the entire data set, which comprises N = n + m observations, the assigned ranks are as follows: 


Observe that if each of these ranks is converted by the formula 2 × rank — 1/2, one gets the following result: 

This corresponds to an assignment of ranks from the Wilcoxon rank- sum statistic when there are N/2 groups of ties, each of size 2.
This means that if An  represents the sum of the ranks of the n treated observations, then under the null hypothesis, the statistic 2An —n/2 has the same distribution as Wilcoxon’s rank-sum statistic Ws*  when there are ℓ = N/2 groups and their sizes are d1  = ··· = dl  = 2.  Therefore, using the formulas seen in class, one finds 

and

where

Accordingly,

8.  Given that the ranks of the treatments are 2, 4, . . . , 2m, one has

Under the null hypothesis, it is known that E(Wr ) = m(2m + 1)/2 = m2 + m/2 and var(Wr ) = m2 (2m + 1)/12. 
When m is sufficiently large, and given that small values of Wr  lead one to reject H0 , one has 

where Z denotes a standard Gaussian random variable. It follows that










         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
