# Hand Gesture Recognition for Sign Language

This project aims to develop an artificial intelligence (AI) model capable of recognizing hand gestures in sign language and translating them into text. The primary objective is to create a tool that enhances communication and interaction for individuals who use sign language as their primary means of communication.

## Key Objectives:
<li>Gesture Recognition: Train a deep learning model to accurately recognize and classify hand gestures commonly used in sign language.</li>
<li>Real-time Translation: Develop the capability to translate recognized gestures into text instantaneously, enabling seamless communication.</li>
<li>User Interface: Create a user-friendly interface that allows users to interact with the system easily, providing both input via gestures and output via text.</li>

## Machine Learning ands Deep Learning Frameworks used:
<li>Tensorflow</li>
<li>Scikit-learn</li>
<li>Numpy,Pandas</li>
<li>Plotly</li>

# Model Architecture


Our model utilizes convolutional layers for feature extraction from hand gesture images, followed by MaxPooling to downsample and preserve key features. Dense layers integrate learned features for gesture classification, enhanced by dropout regularization to prevent overfitting. The final layer employs a sigmoid activation function for multi-label classification, enabling accurate recognition of diverse sign language gestures in real-time applications.


### Optimizers Used:
- RMSprop
- Adam
- Adadelta
- Adagrad

### Results:

|index|Optimizer|Activation Function|Train Loss|Train Accuracy|Train Precision|Train Recall|Val Loss|Val Accuracy|Val Precision|Val Recall|Epoch|
|---|---|---|---|---|---|---|---|---|---|---|---|
|1|Adam|relu|3\.167072296142578|0\.08137045055627823|0\.05069601163268089|0\.6925053596496582|3\.0823893547058105|0\.06793206930160522|0\.05317637324333191|0\.7852147817611694|10\.0|
|0|RMSprop|relu|3\.276334524154663|0\.05781584605574608|0\.039583563804626465|0\.6089935898780823|3\.252866506576538|0\.05494505539536476|0\.03919634968042374|0\.6353646516799927|10\.0|
|2|Adadelta|relu|4\.150864601135254|0\.03768736496567726|0\.03849301114678383|0\.5036402344703674|3\.478652000427246|0\.037962038069963455|0\.03810686990618706|0\.6233766078948975|10\.0|
|3|Adagrad|relu|3\.9087071418762207|0\.05224839225411415|0\.04018346965312958|0\.5177730321884155|3\.3669395446777344|0\.03696303814649582|0\.04011571779847145|0\.41558441519737244|10\.0|

### Activation Functions Tested:
- relu
- sigmoid
- softmax
- tanh
- softsign
- selu
- elu

### Results for RMSprop Optimizer:




|index|Optimizer|Activation Function|Train Loss|Train Accuracy|Train Precision|Train Recall|Val Loss|Val Accuracy|Val Precision|Val Recall|Epoch|
|---|---|---|---|---|---|---|---|---|---|---|---|
|1|RMSprop|sigmoid|3\.4386680126190186|0\.0389721617102623|0\.039464663714170456|0\.5177730321884155|3\.715771198272705|0\.03496503457427025|0\.03822120279073715|0\.3666333556175232|5\.0|
|0|RMSprop|relu|3\.4081802368164062|0\.04796573892235756|0\.04040905833244324|0\.5922912359237671|3\.257030487060547|0\.039960041642189026|0\.038627129048109055|0\.9590409398078918|5\.0|
|5|RMSprop|selu|3\.414308547973633|0\.04282655194401741|0\.03918248787522316|0\.5550321340560913|3\.354295015335083|0\.05294705182313919|0\.038730546832084656|0\.4425574541091919|5\.0|
|3|RMSprop|tanh|3\.4315335750579834|0\.04282655194401741|0\.03871742635965347|0\.5383297801017761|8\.03565788269043|0\.04595404490828514|0\.0|0\.0|5\.0|
|6|RMSprop|elu|3\.403385877609253|0\.04411134868860245|0\.040213149040937424|0\.5558886528015137|12\.560569763183594|0\.03196803107857704|0\.02610441856086254|0\.012987012974917889|5\.0|

## Final Model (RMSprop with relu)

After analyzing different optimizers and activation functions, the model selected for deployment uses RMSprop optimizer with relu activation function based on the following metrics:

- **Train Loss:** 3.244080
- **Train Accuracy:** 0.067666
- **Train Precision:** 0.041408
- **Train Recall:** 0.610707
- **Val Loss:** 3.199470
- **Val Accuracy:** 0.072927
- **Val Precision:** 0.039833
- **Val Recall:** 0.677323

This configuration was chosen for its balanced performance in training and validation phases.



![plot](model.png)
