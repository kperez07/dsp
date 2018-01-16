[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> import nsfg
df = nsfg.ReadFemPreg()
group1=df.loc[df['pregordr'] == 1, 'totalwgt_lb']
group1.mean()
group2=df.loc[df['pregordr'] !=1, 'totalwgt_lb']
group2.mean()
diff = group1.mean() - group2.mean()
import math
var1 = group1.var() 
var2 = group2.var()
n1, n2 = len(group1), len(group2)
pooled_var = (n1 * var1 + n2 *var2)/(n1 + n2)
d = diff / math.sqrt(pooled_var)

Standardized difference between the totalwgt_lb
Cohen's d (mean of 1st baby - mean of more than 1st baby):
d = -0.06911825348820934

Comparison to length: 
d = 0.029
