# Directing Customers to Subscription through App Behaviour Analysis
### Introduction
In today's market, many companies have a mobile presence. Often, these companies provide free products/services in their mobile apps in an attempt to transition their customers to a paid membership. Some examples of paid products, which originate from free ones, are YouTube Premium, Pandora Premium, Audible Subscription, Spotify Premium etc. Since marketing efforts are never free, these companies need to know exactly who to target with offers and promotions.
* __Market:__ The target audience is customers who use a company's free product. In this case study, this refers to users who installed (and used) the companys free mobile app.

* __Product:__ The paid memberships often provide enhanced versions of the free products already given for free, alongside new features. For example, YouTube Premium allows you to leave the app while still listening to a video.

* __Goal:__ The objective of this model is to predict which users will not subscribe to the paid membership, so that greater marketing efforts can go into trying to 'convert' them to paid users.

### Business Problem
In this case study, we will be working for a fintech company that wants to provide its customers with a paid mobile app subscription that will allow them to track all of their finances in one place. To attract customers, the company releases a free version of their app with some of the main features unlocked.

The task is to identify which users will most likely NOT enroll in the paid product, so that additional offers can be given to them. Because of the costs of these offers, the company does not want to offer them to everybody, especially customers who were going to enroll anyway.

### About the dataset
The data allows us to see the date and time of app installation, as well as the features the users engaged with within the app. App behaviour is characterised as the list of app screens the user looked at, and whether the user played the financial mini-games available.

The app usage is only from the user's first day in the app. This limitation exists because users can enjoy a 24-hour free trial of the premium features and the company wants to target them with new offers shortly after the trial is over.

The features are:
* user: The unique user ID
* first_open: The date and time the user joins
* dayofweek: Day of the week in the numerical format (0 is Sunday while 6 is Saturday).
* hour: Hour of the day the app was first opened (same as the time in `first_open`, but only displayed in hours with 24-hr format).
* age: Age of the user.
* screen_list: Every single screen name that the user visited in their 24-hour trial.
* numscreens: No. of screens appearing the screen_list.
* minigame: Whether played the minigame or not (1 is played, 0 is not played).
* like: Every screen has a like button. If the user likes and presses the like button on any of the screen, this gets 1. 0 otherwise.
* used_premium_feature: If the user has used any premium feature in the free trial, this gets 1. 0 otherwise.
* enrolled: Whether the user enrolled for the paid product after the trial. 1 if yes, 0 if no.
* enrolled_date: Date when the user enrolled to the paid product. Only exists when `enrolled` field is 1.

##### Notes about data:
The data for these projects are manufactured fields based on trends in real world case studies. The fields describe what companies usually track from their users, and their distributions are based on observed distributions in real world analysis. This means that, although the data has been artificially ceated, the patterns, associations and distributions are not random.

The data serves as a good representation of what one may encounter in the workplace. That is, the data is rarely clean and a lot of pre-processing is needed to get it ready for modelling.

Dataset courtesy: [SuperDataScience](https://sds-platform-private.s3-us-east-2.amazonaws.com/uploads/P39-CS3-Python-Code.zip)
