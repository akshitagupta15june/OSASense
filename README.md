
<div align="center">
  <h1>OSASense</h1>
<img width="200" height="200" src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/osasense.jpeg">
</div>

</br>


963+ million Number of Patients suffering from Sleep Apnea around the World. Indians are 33% suffering from Sleep Apnea Disorder.As per recent studies NIH and NetMeds India, Indian population is at the high risk of Obstructive Sleep Apnea due to the anatomy, Overweight and Hypertension.

</br>

#### Excessive sleepiness,severe snoring,choking while sleeping are the main symptoms of Sleep Apnea. 
Due to delayed diagnosis, it can lead to chronic and fatal health conditions. Obstructive Sleep Apnea causes Asthma,Diabetes, Hypertension or Heart Attack. Can Also be indicative of ALZHEIMER’S !


#### The pain points include:

1) Difficulty in early diagnosis leading to surgical complications.
2) Hectic procedures at the Sleep Labs and most importantly Delayed diagnostic.
3) less availability approx 500 sleep labs.
4) Smoking can increase the amount of inflammation and fluid retention in the upper airway. 


</br>

## What is OSASense?

```
A Screening solution for Obstructive Sleep Apnea that also helps us to 
monitor the severity of the disease using ML and mobile application.
Prediction of the severity of obstructive sleep apnea
by anthropometric features via support vector machine(SVM). 
```

</br>

<div align="center">
<img src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/sleepl.jpeg">
</div>

</br>

## Our Application Flow-:

1) It’s pretty handy to use. The patient clicks on the app.

2) Answers a few simple questions and on the basis of that you get a report whether or not you have sleep apnea.

3) We are using Machine Learning(SVM) algorithm for finding out the AHI(The apnea-hypopnea index), a scale that tells whether or not you have Sleep Apnea and how severe it is.



## Technical Requirements:

1) Google Collab GPU: Tesla T4 (compute capability: 7.5 ITR/SEC)

2) Dataset of sleep labs: [SLEEP-DATA](https://github.com/akshitagupta15june/OSASense/blob/main/Sleep-lab-Dataset/sleeep_apnea_data.xlsx), [SLEEP-SET](https://github.com/akshitagupta15june/OSASense/blob/main/Sleep-lab-Dataset/sleep-set.xlsx)

The dataset of Patients information was collected from two independent sleep centres at the Taipei Medical University Hospital (TMUH, Taipei, Taiwan)
and Shuang-Ho Hospital (SHH, New Taipei City, Taiwan).The inclusion criteria for this study were patients referred for suspected sleep disordered breathing, ages between 20 and 80.

Sample Image of the dataset

<img src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/datset.jpeg">



</br>

```
AHI: Apnea hypopnea index we have considered that if AHI is greater than 15 and less than 30
then the person has no sleep apnea but if the AHI is greater than 30 then the person is positive with sleep apnea. 
```
</br>

<img height="150" width="450" src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/ahi.png">

</br>

## Approach of solution

We apply a modern machine learning method, the support vector machine and TensorFlow (open-source software library) to establish a predicting model for the severity of OSA. 


we establish a prediction model for Asians by taking body shape profiles and age into account via SVM.
We hypothesize that the established predictors are accurate for OSA severity. To confirm this hypothesis, 
we collected two large patient databases from two independent sleep labs and designed a prediction model for the OSA severity based on body shape profiles. 

We randomly partitioned the data into the training dataset and the testing dataset, with the training dataset being created by randomly selecting 20% of the patients while the remainder serving as the testing dataset.

###### Positive (1) and negative (0) results of patients are predicted in our model:


<img src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/positive.jpg">
<img src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/negative.jpg">

Age, sex, weight and height, Epworth Sleepiness Scale (ESS), BQ (Behavioural Quotient). Furthermore, the anthropometric features such as head, buttock, waist and neck circumferences were also measured in the sleep lab. 


</br>

<img src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/acc.jpg">


The BQ is composed of three categories including snoring behaviour, waketime sleepiness or fatigue, and obesity and/or hypertension. Each of these categories is classified as severe or not severe. If two out of three categories are severe, then the patient is of high risk with BQ number 1; otherwise the patient is of low risk with BQ number 0.

</br>

<img src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/accuracy.jpg">

#### The accuracy was approximately 77.02% by using SVM. As the accuracy by SVM was low so we used TensorFlow. TensorFlow is a free and open-source software library for dataflow and differentiable programming across a range of tasks. We have used tf.keras, a high-level API to build and train the model in TensorFlow and we got accuracy of 86.4%.

When we add a new dataset in the previous one so the accuracy for increased.


#### APP MOQUPS


##### These are app moqups. 
##### The suspected patient logs in. He’s required to answer questions of BQ like Snoring behaviour, obesity etc. 


<img height=400 width=700 src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/mo1.png">

##### Followed by Epworth Sleep Scale and finally Anthropometric measures like Neck Size, Buttok Size, BMI.
</br>
<img height=400 width=700 src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/mo2.png">
</br>


#### On the basis of this information, ML algorithms  will calculate AHI by taking reference from the data of the diseased population procured at backend from the Sleep labs. The final result will be a predictive analysis. 

<img height=300 width=250 src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/5.png">


##### The patient will be notified and about the nearby sleep lab and he/she can go for further check ups.


<img height=400 width=200 src="https://github.com/akshitagupta15june/OSASense/blob/main/Images/map.jpg">



A better understanding of these will help in the development of novel therapies. Further research is also needed to identify biomarkers for patients at risk for consequences of OSA as well as predictors for treatment success to enable the development of individual therapeutic approaches for the implementation of personalized medicine.


### References:

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4739955/

https://www.resmed.co.in/blogs/prevalence-sleep-apnea-india

https://www.lungindia.com/article.asp?issn=0970-2113;year=2018;volume=35;issue=4;spage=301;epage=306;aulast=Pinto

### Team 

Akshita Gupta

Tanvi Balaiwar

Anamika Pal


