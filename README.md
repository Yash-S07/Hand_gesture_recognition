# Hand Gesture Recognition: 
Hand Gesture Recognition for Sign Language
This project aims to develop an AI model capable of recognizing hand gestures in sign language and translating them into text. The goal is to facilitate communication and interaction for individuals who use sign language.

Optimizers Comparison
Optimizers Used:
RMSprop
Adam
Adadelta
Results:
Epochs	Optimizer	Activation Function	Train Loss	Train Accuracy	Train Precision	Train Recall	Val Loss	Val Accuracy	Val Precision	Val Recall
8	9	Adadelta	relu	4.202672	0.031692	0.038538	0.500214	3.374346	0.037962	0.040084
7	8	Adam	relu	3.311365	0.051820	0.042833	0.553319	3.246309	0.053946	0.042254
0	1	Adadelta	relu	4.181376	0.043255	0.037815	0.494218	3.331768	0.041958	0.038890
6	7	Adam	relu	3.326572	0.050964	0.042110	0.537473	3.272782	0.035964	0.040731
8	9	RMSprop	relu	3.244080	0.067666	0.041408	0.610707	3.199470	0.072927	0.039833
Activation Function Analysis
Activation Functions Tested:
relu
sigmoid
softmax
tanh
softsign
selu
elu
Results for RMSprop Optimizer:
Epochs	Optimizer	Activation Function	Train Loss	Train Accuracy	Train Precision	Train Recall	Val Loss	Val Accuracy	Val Precision	Val Recall
9	10	RMSprop	softsign	3.262897	0.044968	0.039963	0.589722	3.475484	0.040959	0.023810
9	10	RMSprop	sigmoid	3.240383	0.060814	0.041611	0.605567	5.251967	0.035964	0.033548
5	6	RMSprop	selu	3.370477	0.039400	0.040016	0.555889	3.253613	0.048951	0.039661
0	1	RMSprop	softmax	3.959502	0.044111	0.038332	0.496788	3.314115	0.043956	0.040493
8	9	RMSprop	softmax	3.309988	0.044111	0.039247	0.473233	3.339227	0.041958	0.000000
Final Model (RMSprop with relu)
After analyzing different optimizers and activation functions, the model selected for deployment uses RMSprop optimizer with relu activation function based on the following metrics:

Train Loss: 3.244080
Train Accuracy: 0.067666
Train Precision: 0.041408
Train Recall: 0.610707
Val Loss: 3.199470
Val Accuracy: 0.072927
Val Precision: 0.039833
Val Recall: 0.677323
This configuration was chosen for its balanced performance in training and validation phases.

![plot](model.png)
