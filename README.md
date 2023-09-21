# Mobile-price-prediction

![image](https://user-images.githubusercontent.com/82583885/222394483-e56d9b2e-c44b-47aa-913b-48f49994b143.png)

In the competitive mobile phone market companies want to understand sales data of mobile phones and the factors which drive the prices. The objective is to find out some relation between the features of a mobile phone(e.g.:- RAM, Internal Memory, etc.) and its selling price. In this problem, we do not have to predict the actual price but a price range indicating how high the price is.

📱This notebook includes the following:

* Preprocessing
* Data cleaning
* Exploratory data analysis (EDA)
* Preparing the data to train a model
* Training and making predictions using various classification models
* Model evaluation
* Model Explainability


# **Data Description**
Battery_power - Total energy a battery can store in one time measured in mAh

Blue - Has Bluetooth or not

Clock_speed - speed at which microprocessor executes instructions

Dual_sim - Has dual sim support or not

Fc - Front Camera megapixels

Four_g - Has 4G or not

Int_memory - Internal Memory in Gigabytes

M_dep - Mobile Depth in cm

Mobile_wt - Weight of mobile phone

N_cores - Number of cores of processor

Pc - Primary Camera megapixels

Px_heig Px_height - Pixel Resolution Height

Px_width - Pixel Resolution Width

Ram - Random Access Memory in MegaBytes

Sc_h - Screen Height of mobile in cm

Sc_w - Screen Width of mobile in cm

Talk_time - longest time that a single battery charge will last

Three_g - Has 3G or not

Touch_screen - Has touch screen or not

Wifi - Has wifi or not

Price_range - This is the target variable with values of 0(low cost), 1 (medium cost), 2(high cost) and 3(very high cost).

# **" Where there is DATA SMOKE, there is BUSINESS FIRE. " - Thomas Redman**

# **The models implemented are:**

* K Nearest Neighbour

* Naive Bayes Classifier(Gaussian Naive Bayes)

* Decision Tree Classifier

* Random Forest Classifier

* Extreme Gradient Boosting Classifier

# **Conclusion**

## Conclusion from EDA:

* Clock speed , front camera , pixel height and screen width are right skewed distributed. Other variables are not skewed.

* 1010 have bluethooth while 990 do not have bluetooth.(50% have bluetooth)

* 1019 mobile phones are dual sim while 981 are single sim (50% are dual sim phones).

* 1043 are 4g devices while 957 devices do not support 4g (52% devices support 4g)

* 1523 are 3g devices while in 477 devices 3g is not supported (More than 75% devices support 3g).

* 1006 are touch screen phones while 994 are keypad phones. (50% are touch screen).

* 1014 devices support wifi while 986 devices do not support wifi (Wifi is avaiilable on half of the devices).

* All the processors have equal number of devices (No of cores are eually distributed, from 12-13% for all cores).

* Price_range have equal distribution (each price range from low to very high have equal numbers of records). Hence it is perfectly balanced dataset.

* Here front caamera has some outliers but other outliers are not seen much.

* Battery power do not affect the price range much.

* Ram is highly affecting the price of mobile.

* Non bluetooth mobile phones with higher price are less in number but phones with bluetooh are available in all price range.

* Phones without double sim have low price while phones with double sim are available in all price range.

* Prices of non 4g phones are lower but price of 4g phones are ranges from low to very high.

* There are larger number of 3g phones but their prices do not vary much.

* Touch screen phones are available in all price range.

* Phones with wifi facility are available in all price range.

* If primary camera quality is good then front camera quality is also good.

* When the device is not 3g then there is no record that it is 4g. Hence it is neccesary for a 4g mobile phone that it must be 3g.

* If there is low pixel pixel width then pixel height can be low but cannot be high. There can be lower pixel heights at high pixel width.

## Conclusion from Modelling:
Among all the models implemented, XGBoost classifier is performing the best since it gives highest accuracy for train and test dataset. Hence to deploy the model, XGB can be used for final prediction of mobile price range.
