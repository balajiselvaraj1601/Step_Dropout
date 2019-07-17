# Step_Dropout
Using Step dropout to improve accuracy of modified NIN network on CIFAR 100

Adaptive Dropout:
This is an approach which i tried for carrying out step by step increase of dropout rate.
The value of dropout increase with number of epoch.
It reaches the maximum value of 0.5 at the last epoch
File:

https://github.com/balajiselvaraj1601/Step_Dropout/blob/master/Adaptive_Dropout_NIN_CIFAR100_final.ipynb

Non-Adaptive Dropout:
The value of dropout is fixed and does not change
File:

https://github.com/balajiselvaraj1601/Step_Dropout/blob/master/No_Adaptive_Dropout_NIN_CIFAR100_final.ipynb

Curriculum dropout (annealing) is unofficial implementation of the paper

https://arxiv.org/abs/1703.06229

Official implementation can be found in the following link
https://github.com/pmorerio/curriculum-dropout

Curriculum (line drop) 
This is an approach that I tried having properties similar to curriculum annealing and adaptive dropout

|Technique	            | train_loss	| valid_loss	| accuracy |	error_rate	| top_k_accuracy |
|-----------------------|-------------|-------------|----------|--------------|----------------|
|Adaptive	              |  2.445148	  |  1.571715	  |  0.5796	 |    0.4204	  |   __0.8477__   |
|Non-Adaptive	          |  2.478166	  |  1.655046 	|  0.5577	 |    0.4423  	|     0.8336     |
|Curriculum (Annealing) |__2.206255__ |__1.5655344__|__0.5837__|  __0.4163__  |     0.8473     |
|Curriculum (Line drop) |  2.461889	  |  1.599115	  |  0.5712	 |    0.4288	  |     0.8442     |


Testing is done on modified NIN architecture. Results are shown only for it.
Further analysis is under progress
Try it and kindly share your suggestions and views

Next Steps:
To Setup Curriculum dropout
