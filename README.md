# Step_Dropout
Using Step dropout to improve accuracy of modified NIN network on CIFAR 100

Adaptive Dropout:
The value of dropout increase with number of epoch.
It reaches the maximum value of 0.5 at the last epoch
File:
https://github.com/balajiselvaraj1601/Step_Dropout/blob/master/Adaptive_Dropout_NIN_CIFAR100_final.ipynb

Non-Adaptive Dropout:
The value of dropout is fixed and does not change
File:
https://github.com/balajiselvaraj1601/Step_Dropout/blob/master/No_Adaptive_Dropout_NIN_CIFAR100_final.ipynb

|Technique	| train_loss	| valid_loss	| accuracy |	error_rate	| top_k_accuracy |
|-----------|-------------|-------------|----------|--------------|----------------|
|Adaptive	    | 2.445148	|  1.571715	  |  0.5796	 |    0.4204	  |       0.8477   |
|Non-Adaptive	| 2.478166	|  1.655046 	|  0.5577	 |    0.4423  	|       0.8336   |

Testing is done on modified NIN architecture. Results are shown only for it.
Further analysis is under progress
Try it and kindly share your suggestions and views

Next Steps:
To Setup Curriculum dropout
