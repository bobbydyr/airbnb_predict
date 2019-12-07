# AirBnb Listing Price Prediction from Scratch

- Focused on Feature Engineering methods, and the whole model were developed from scratch. 


**Link** -> https://github.com/bobbydyr/airbnb_predict/blob/master/airbnb_prediction.ipynb

![](/pic/fomular1.png)

## Goal:
- This project is primarily the goal to build a mutiple linear regression to predict housing price.

1. Feature Engineering.
2. Build model with regression fomular.
3. Interpret model.
![](/pic/pic1.png)

## Executive Summary:

**(a) AirBnB hosts**
- Prospective AirBnB hosts could potentially use our model to predict certain rooms/spaces of their own before making the decision to re-purpose them for AirBnB. Since our model can predict to some accuracy the prices of their spaces, they could use the model to predict how much money they will make. Therefore, if they are debating whether or not they should rent their places via AirBnB, they now have the extra information to aid their decision-making process.

- For current AirBnB hosts, our model can also aid them in deciding how much they should charge for their places. The hosts can use our model to predict how much some certain places will be charged on AirBnB. They can use this information to price their listings in a price range they are confident in.

**(b) AirBnB customers**
- As for AirBnB customers, I think our model is best used for them to verify the pricing of certain listings that they are interested in renting. For example, it may be hard for customers to compare the pricing of listings in an area where AirBnB listings are scarce. I.e., they may not be able to see similar listings within an area and thus may not be able to tell whether or not the lisitng they are looking at is priced fairly or not. Our model can help them to predict the pricing of the listing. If the listing is **significantly more expensive** than our prediction, it is worth considering the listing may be over-priced and vice versa.

**(c) Interesting Predictors**
1. Negative factors on price:
    1. has_availability: This is really interesting, but we could think about it this way. A listing is avaliable maybe because nobody wants to rent it.
    2. room_type_Shared room: This is intuitive. Like carpools, shared rooms would be cheaper.
    3. beds: this is intuitive because more beds usually means more expenses.
    4. The price drops when it is located in University district. And This is intuitive as well, students are poor.
2. Positive factors on price:
    1. requires_license: One way to understand this is, if a listing requires license, it may be because the house is expensive, and the househost does not want accomendate some random people with no reliable background info.
    2. bedrooms: This is to be expected. The larger the space is, the more it will likely to cost.

## Steps for feature engineering:
- Step 0: Select features, filter out text and irrelavent features.
- Step 1: Change text to float numbers using regex
- Step 2: Normalize: (x - mean) / standard deviation
- Step 3: Calculate how many days has been hosted, difference for date
- Step 4: Ordinal variable to numerical numbers.
- Step 5: Boolean value to 0/1.
- Step 6: One-hot-encoding
- Step 7: Change 80% -> 0.8
- Step 8: Input na with mean
- Step 9: Drop some na instances.
- Step 10: Drop outliers. (3 standard deviations away from mean.)
- Step 11: Drop the observation where price = 0.
- Step 12: Give a log to label, since price is really skewed. 








