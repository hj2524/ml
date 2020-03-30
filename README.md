# Project: Can you recognize the emotion from an image of a face? 
<img src="figs/CE.jpg" alt="Compound Emotions" width="500"/>
(Image source: https://www.pnas.org/content/111/15/E1454)

### [Full Project Description](doc/project3_desc.md)

Term: Spring 2020

+ Team # 5
+ Team members
	+ Zhao, Ziqin zz2709@columbia.edu
	+ Liu, Jiawei jl5560@columbia.edu
	+ Chen, Shenghan sc4615@columbia.edu
	+ Yu, Tianning ty2422@columbia.edu
	+ Konte, Marko mk4222@columbia.edu

[Presentation file here](https://github.com/TZstatsADS/Spring2020-Project3-group5/blob/master/doc/Project%203-%20Image%20Classification.pptx)

+ **Project summary:** 
In this project, we created a classification engine for facial emotion recognition. The goal of this model was to accurately predict an emotion shown from a facial image. We started from a baseline model using the gradient boosting method and then tested several different model approaches for our advanced model. Ultimately, the best performing advanced model was creating Neural Network. This was closesly followed by the Ensemble model. 

	+ **Baseline:** The gradient boosting function, GBM, was used with 
		+ Test Accuracy: 38.20%
		+ Model  Time: 9 minutes.
		+ Training Accuracy: 83.8%
	
	+ **Advanced:** Neural Network using functions from the keras and tensorflow packages, had the best results of all tested 				models. This type of model takes a collection of inputs which are processed within the hidden layer to find 				useful connection points, before being distributed in the output layer as classification prediction.  
		+ Test Accuracy: 58% 
		+ Model Time: 11.24 Minutes. 
		+ Training Accuracy: 94.60%
	
	+ *Other Attempted Advanced Models:*
		+ Ensemble: The very close second best performer after the Neural Network. This type of model allows for combining 				multiple model results to improve the end classification. In our model we used the Voting method for the 				ensemble model to make the final combination using Logistic Regression, LDA, and SVM Methods.  
			+ Test accuracy: 54.60
			+ Model time: 3.07 Minutes
		+ XGBoost: Reached test accuracy of 49.2% within a time of 17.76 seconds. 
		+ Logistic Regression: Reached test accuracy of 51.2% within a timee of 40 seconds. 
		+ SVM: Reached testing accuracy of 48.4% within a time of 55 seconds. 
		+ LDA: Reached testing accuracy of 53.8% within a time of 2.22 minutes. 
		+ Random Forest: Reached testing accuracy of 43.0% within a time of 11.24 seconds.

**Contribution statement**: ([default](doc/a_note_on_contributions.md)) All team members contributed equally in all stages of this project. All team members approve our work presented in this GitHub repository including this contributions statement. 

*Ziqin Zhao* Created baseline model, NN model, and put together the final Main notebook. 

*Jiawei Liu*

*Shengham Chen*

*Tianning Yu*

*Marko Konte* Created the LDA, tested different iterations of NN, and tested all models considered using optimized feature sets. Also created the presentation and the READ.me file 

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
