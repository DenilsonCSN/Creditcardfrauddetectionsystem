<h1>Machine Learning-based Credit Card Fraud Detection System</h1>

<h2>Description</h2>
As we are moving towards the digital world cyber security is becoming very important for our lives, we make lots of purchases online and a good amount of people prefer credit cards. Using credit card limits sometimes helps people to complete transactions even if they don’t have the amount at the time and this makes people vulnerable to cyber attackers.
The importance of this project is to tackle the issue by designing a system that can find abnormal activity and abort the transaction if it is fishy or suspicious a system that can track the pattern of all transactions.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Machine learning</b>
- <b>Python</b>


<h2>Environments Used </h2>

- <b>GoogleColab</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Dataset: <br/>
<img src="https://i.imgur.com/dcHWf18.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Importing the necessary Libraries:  <br/>
<img src="https://i.imgur.com/dKN74z5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Importing The Dataset: <br/>
<img src="https://i.imgur.com/ms3g2md.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Data Processing and Understanding:  <br/>
<img src="https://i.imgur.com/HHx92xo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Check for null values using the following code:  <br/>
<img src="https://i.imgur.com/gbMTaPu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
No null values according to the count per column. Additionally, this use case does not include feature selection. In any case, you can test whether the results are optimised by using feature selection procedures in this data, I've seen that 28 characteristics are PCA-transformed copies, but the amount is still the original and while verifying the amount's minimum and maximum, I discovered a significant variation that could affect our outcome.:  <br/>
<img src="https://i.imgur.com/KsPtWZf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Scaling this variable in this situation is a good idea. To fix it, we can utilise a common scaler.:  <br/>
<img src="https://i.imgur.com/dyvhhwO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
We still have one additional variable the time which may operate as an outside deciding factor, but we can ignore it for the purposes of our modelling method. Also, we'll look for any transactions that have already occurred. We currently have 284807 transactions in our data before any duplicate ones are removed. Let's get rid of the duplicate and see the results:  <br/>
<img src="https://i.imgur.com/HIv5Ul5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
By running the bellow line of code, we can remove any duplicate left and by running the “. shape” command we can check the results again:  <br/>
<img src="https://i.imgur.com/zkjFNtL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
Training and Test Split:  <br/>
<img src="https://i.imgur.com/4R4IGJH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
Next let’s split the train and test data:  <br/>
<img src="https://i.imgur.com/tLvGVrP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Model Building:  <br/>
<img src="https://i.imgur.com/MlI2WLs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The machine learning model that will be utilised in the project is defined by this block of code:  <br/>
<img src="https://i.imgur.com/grTmZ5B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Logistic regression:  <br/>
<img src="https://i.imgur.com/MQvohQs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
XGBoost:  <br/>
<img src="https://i.imgur.com/Y1q3Y54.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
SVM:  <br/>
<img src="https://i.imgur.com/yd7XIbE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Random Forest:  <br/>
<img src="https://i.imgur.com/eBL5sQ1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
