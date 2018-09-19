[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

```python

def CohenEffectSize(group1, group2):
	
    diff = group1.mean() - group2.mean()

    var1 = group1.var()
    var2 = group2.var()
    n1, n2 = len(group1), len(group2)

    pooled_var = (n1 * var1 + n2 * var2) / (n1 + n2)
    d = diff / np.sqrt(pooled_var)
    return d
    

firsts = live[live.birthord == 1]
others = live[live.birthord != 1]
 
firsts.totalwgt_lb.mean() 
others.totalwgt_lb.mean()

CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)
```
Mean of total weight of first babies: 7.201094430437772    
Mean of total weight of other babies: 7.3258556149732623    
Difference of means: -0.12476118453549034   
Cohen's d = -0.088672927072602006   

The difference in means is -0.088 standard deviations, which is small. In comparison the difference in pregnancy lenght which has effect size 0.028, the difference in weights is more significant. 
