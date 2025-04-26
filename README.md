# comp9414-assignment-1---artificial-neural-networks-solved



**<span style='color:red'>TO GET THIS SOLUTION VISIT:</span>** https://www.ankitcodinghub.com/product/comp9414-24t2-solved/

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;131255&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP9414 Assignment 1 - Artificial neural networks Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">
            
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
    
<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
Artificial Intelligence

Assignment 1 – Artificial neural networks

1 Problem context

Time Series Air Quality Prediction with Neural Networks: In this assignment, you will delve into the realm of time series prediction using neural network architectures. You will explore both classification and estimation tasks using a publicly available dataset.

You will be provided with a dataset named “Air Quality,” [1] available on the UCI Machine Learning Repository . We tailored this dataset for this assignment and made some modifications. Therefore, please only use the attached dataset for this assignment.

Table 1: Variables within the dataset.

Variable Meaning

CO(GT) True hourly averaged concentration of carbon monoxide

PT08.S1(CO) Hourly averaged sensor response

NMHC(GT) True hourly averaged overall Non Metanic HydroCarbons concentration

C6H6(GT) True hourly averaged Benzene concentration

PT08.S2(NMHC) Hourly averaged sensor response

NOx(GT) True hourly averaged NOx concentration

PT08.S3(NOx) Hourly averaged sensor response

NO2(GT) True hourly averaged NO2 concentration

PT08.S4(NO2) Hourly averaged sensor response

PT08.S5(O3) Hourly averaged sensor response

T Temperature

RH Relative Humidity

AH Absolute Humidity

2 Activities

This assignment focuses on two main objectives:

• Classification Task: You should develop a neural network that can predict whether the concentration of Carbon Monoxide (CO) exceeds a certain threshold – the mean of CO(GT) values – based on historical air quality data. This task involves binary classification, where your model learns to classify instances into two categories: above or below the threshold. To determine the threshold, you must first calculate the mean value for CO(GT), excluding unknown data (missing values). Then, use this threshold to predict whether the value predicted by your network is above or below it. You are free to choose and design your own network, and there are no limitations on its structure. However, your network should be capable of handling missing values.

• Regression Task: You should develop a neural network that can predict the concentration of Nitrogen Oxides (NOx) based on other air quality features. This task involves estimating a continuous numerical value (NOx concentration) from the input features using regression techniques. You are free to choose and design your own network and there is no limitation on that, however, your model should be able to deal with missing values.

In summary, the classification task aims to divide instances into two categories (exceeding or not exceeding CO(GT) threshold), while the regression task aims to predict a continuous numerical value (NOx concentration).

2.1 Data preprocessing

It is expected you analyse the provided data and perform any required preprocessing. Some of the tasks during preprocessing might include the ones shown below; however, not all of them are necessary and you should evaluate each of them against the results obtained.

(a) Identify variation range for input and output variables.

(b) Plot each variable to observe the overall behaviour of the process.

(c) In case outliers or missing data are detected correct the data accordingly.

(d) Split the data for training and testing.

2.2 Design of the neural network

You should select and design neural architectures for addressing both the classification and regression problem described above. In each case, consider the following steps:

(a) Design the network and decide the number of layers, units, and their respective activation functions.

(b) Remember it’s recommended your network accomplish the maximal number of parameters Nw &lt; (number of samples)/10.

(c) Create the neural network using Keras and TensorFlow.

2.3 Training

In this section, you have to train your proposed neural network. Consider the following steps:

(a) Decide the training parameters such as loss function, optimizer, batch size, learning rate, and episodes.

(b) Train the neural model and verify the loss values during the process.

(c) Verify possible overfitting problems.

2.4 Validating the neural model

Assess your results plotting training results and the network response for the test inputs against the test targets. Compute error indexes to complement the visual analysis.

(a) For the classification task, draw two different plots to illustrate your results over different epochs. In the first plot, show the training and validation loss over the epochs. In the second plot, show the training and validation accuracy over the epochs. For example, Figure 1 and Figure 2 show loss and classification accuracy plots for 100 epochs, respectively.

Figure 1: Loss plot for the classifica- Figure 2: Accuracy plot for the clas-

tion task sification task

Table 2: Confusion matrix for the test data for the classification task.

Confusion Matrix Positive (Actual) Negative (Actual)

Positive (Predicted) 103 6

Negative (Predicted) 6 75

Table 3: Accuracy and precision for the test data for the classification task.

Accuracy Precision Number of Samples

CO(GT) classification 63% 60% 190

(c) For the regression task, draw two different plots to illustrate your results. In the first plot, show how the selected loss function varies for both the training and validation through the epochs. In the second plot, show the final estimation results for the validation test. For instance, Figure 3 and Figure 4 show the loss function and the network outputs vs the actual NOx(GT) values for a validation test, respectively. In Figure 4 no data preprocessing has been performed, however, as mentioned above, it is expected you include this in your assignment.

(d) For the regression task, report performance indexes including the Root Mean Squared Error (RMSE), Mean Absolute Error (MAE) (see a discussion on [2]), and the number of samples for your estimation of

Figure 4: Estimated and actual NOx(GT) for the validation set.

Figure 3: Loss plot for the regression task.

NOx(GT) values in a table. Root Mean Squared Error (RMSE) measures the differences between the observed values and predicted ones and is defined as follows:

, (1)

where n is the number of our samples, Yi is the actual label and Yˆi is the predicted value. In the same way, MAE can be defined as the absolute average of errors as follows:

. (2)

Table 4: Result table for the test data for the regression task.

RMSE MAE Number of Samples

90.60 50.35 55

3 Testing and discussing your code

For marking your results, you should be prepared to simulate your neural model with a generalisation set we have saved apart for that purpose. You must anticipate this by including in your submission a script ready to open a file (with the same characteristics as the given dataset but with fewer data points), simulate the network, and perform all the validation tests described in Section 2.4 (b) and (d) (accuracy, precision, RMSE, MAE). It is recommended to save all of your hyper-parameters and weights (your model in general) so you can call your network and perform the analysis later in your discussion session.

3. Fair, 2. Low, 1. Deficient, 0. No answer.

Results obtained with given dataset

Performance indexes table for regression task 1 mark

Results obtained with generalisation dataset

Code understanding and discussion

Code readability for classification task 1 mark

Code readability for regression task 1 mark

Code understanding and discussion for classification task 5 mark

Code understanding and discussion for regression task 5 mark

4 Submitting your assignment

Although we try to answer questions as quickly as possible, we might take up to 1 or 2 business days to reply, therefore, last-moment questions might not be answered timely.

References

[1] De Vito, S., Massera, E., Piga, M., Martinotto, L. and Di Francia, G., 2008. On field calibration of an electronic nose for benzene estimation in an urban pollution monitoring scenario. Sensors and Actuators B: Chemical, 129(2), pp.750-757.
