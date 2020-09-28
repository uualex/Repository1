# Project 2

## Part 1 Population Changes

Population Increase 2010-2014
![](Populationincrease.png)

Average Growth Rate 2010-2014
![](averagegrowthrate.png)

## Part 2 Stock Predictor

Model 1 
~~~
> model_RCL <- buildModel(specs_RCL, method="lm",
+                        training.per=c('2020-02-10' , ' 2020-9-10'))
> summary(model_RCL)

quantmod object:   lm1601258039.17314 	Build date:  2020-09-27 21:53:59 

Model Specified: 
     Next(Cl(RCL)) ~ Cl(CCL) 

Model Target:  Next.Cl.RCL 		 Product:  RCL 
Model Inputs:  Cl.CCL 

Fitted Model: 

	Modelling procedure:  lm 
	Training window:  149  observations from  2020-02-10 to 2020-09-10

Call:
lm(formula = quantmod@model.formula, data = training.data)

Residuals:
     Min       1Q   Median       3Q      Max 
-31.6160  -6.3631  -0.4652   5.5236  20.1998 

Coefficients:
            Estimate Std. Error t value Pr(>|t|)    
(Intercept)  15.6593     1.9936   7.855 7.74e-13 ***
Cl.CCL        2.1254     0.1009  21.065  < 2e-16 ***
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 10 on 147 degrees of freedom
Multiple R-squared:  0.7512,	Adjusted R-squared:  0.7495 
F-statistic: 443.8 on 1 and 147 DF,  p-value: < 2.2e-16
~~~

Model 2 
![](RCL_model2.txt)

Model 3 
![](RCL_model3.txt)
