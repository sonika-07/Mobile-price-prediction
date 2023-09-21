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
