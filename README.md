# INFO 370 Final Project
## Project Description
### What is the overarching purpose of your research project, and why is it an important undertaking?
There are many apps currently on the market. While some applications are popular, others are not. We wanted to determine what factors play a role in an application’s popularity and thus predict an application's popularity based upon it. This task is important as it allows developers and companies to determine the best possible application to create in order to create a widely used application. Our findings will even the playing field for companies/entrepreneurs attempting to break into the mobile gaming industry by providing knowledge of what makes a successful application, as well as provide students interested in the gaming industry with an understanding of what makes an app popular. Furthermore, we are helping users of gaming apps because by openly sharing what makes a gaming app competitive in an open market, companies will pick up on this and users will have a more competitive market of gaming apps to choose from. 

Our model will attempt to predict how different combinations of names, ratings, updates, payment model, cost, genres and categories will impact our users. This will allow developers to know what characteristics will make for the best basic app model, even before they have finished development. Although our research won't guarantee success by using the best app-models we find and report on, it can allow developers and business people to set themselves up for success.

### How does your research fit into the broader problem domain? You should cite at least 3 papers that help contextualize your research. 

The broader problem domain is determining the probability of an application making a profit. Our research focuses on whether an application will be popular because if we can determine whether an application will be popular, there will be a greater chance of it making a profit for the developers/companies, and in return, we create business knowledge that is helpful for the gaming industry as a whole. From our research, we have learned that applications who have more recent updates tend to be more popular as well as target demographics having a greater impact on popularity. We also gained insight that certain app rating affects the popularity of the app, as it targets different audiences. Technologies used also has an influence on the popularity of an app, as visual stimulation and fast-rendering is directly related to the technologies used to create the app. Through the analysis we may be able to determine for example maturity-rating may be one of the most important factors and what rating one should aim for to make a successful application.

Interestingly, one study found that "a changing app price does not correlate with the download count". It seems that a changing app price won't negatively affect user downloads as may be expected, so our research can now enter in and determine what the best models to change, or start with, might be (1). In addition, there are studies that show a user's demographics can be predicted with a degree of accuracy based on the types of apps they have downloaded, so we know that certain aspects of apps on the Google Play store can be predicted using machine learning (2). It will also be interesting to see how our findings on the most effective categories for apps are when combined with research on what the most popular categories to develop for are(5). For instance, Education apps are the most common type of app on the Google Play store, but does that neccesarily imply it's the best choice to start developing an app for? After all, it may be easier to make an impact in the smallest category, Music, but maybe there is a reason so few developers choose to embrace the challenge of a music app.

Sources:
* (1) https://arxiv.org/pdf/1802.02996.pdf
* (2) https://arxiv.org/pdf/1603.00059.pdf
* (3) http://www.pewinternet.org/2015/11/10/an-analysis-of-apps-in-the-google-play-store/
* (4) https://www.newgenapps.com/blog/steps-successful-mobile-game-development
* (5) http://www.businessofapps.com/data/app-statistics/

### What specific hypothesis (hypotheses) are you going to test?
If a developer/company follows the current trends, creating an application with similar features as the most popular apps, then the app will have more installs because it appeals to a broader audience.

Including certain words or combinations of words in the title of an app will have a significant effect on the downloads and reviews of an app.

### What are the datasets you'll be working with to answer this question? Please include relevant background describing the datasets you identify.
The dataset we will be working within this research project was web scraped by a user on Kaggle at:
* https://www.kaggle.com/lava18/google-play-store-apps
The dataset holds information such as maturity-rating, payment-model, applications size, etc.

### What statistical and machine learning methods do you plan on using to test your hypothesis?
We plan to use a few methods, some of which are: multiple linear regressions, univariate analysis, and bivariate analysis. Specifically we expect to use multiple Ordinary Least Regressions, most likely including forward or backward selection, to determine a baseline of the effect that different features of an app have on the model.

After this, we plan to use multiple machine learning methods to make a model that can predict any given app's success. The features we have are limited so it may only reach a certain level of accuracy, but it can set a baseline for what developers can expect from a certain app. The "name" feature is something we are particularly interested in because it doesn't seem like a lot of research has been done on the impact the title of an app has on it's download success. This seems like an area that would be important though, since a title is the first and sometimes only sales pitch an app will get.

A few of the machine learning models we plan to use to test our hypothesis are: Principal Component Analysis, because it will be effective especially initially in showing us which features are most important to an app's "success", and it will help us narrow down all of our categorical features in the dataset. In order to get an idea of the broad types of apps out there we will consider using a "k-means" approach, although this may be challenging due to the size of our dataset, according to the Python Data Science Handbook though this can still be an effective method with a subset of the data. For supervised methods, we plan to use regression via sklearn as well as Support Vector Machines. Support vector machines will be an effective way to predict the data, while linear/polynomial regression will be more easily interpretable.

### Who is your target audience for the resource you will build? Depending on the domain of your data, there may be a variety of audiences interested in using the dataset. You should hone in on one of these audiences.
The target audience in our research projects would be individual developers/companies as they want to create an application with the best chance of mainstream success.

### What should your audience learn from your resource? Consider specific questions they may want to answer.
The audience would learn from the resource is: “what type of application would be best to create” or at least, which types of applications will give them better chances of succss. That is based upon the application’s TITLE, pay-model, genre, maturity rating, etc; we wanted to determine which factors the most into an application’s success. Or “will making my application pay-to-use decrease its popularity?” 

## Technical Description
### What will be the format of your final web resource (Shiny app, HTML page or slideshow compiled with KnitR, etc.)?
A Jupyter Notebook created HTML page report, hosted on GitHub pages.

### Do you anticipate any specific data collection/data management challenges?
There may be duplicate entries for the same application, we’re going to need to clean this up if that is the case. The dataset is pretty huge, this may cause technical issues, we might need to run our analysis on a third of the dataset as opposed to the whole dataset at any given time.

Our approach for machine learning will also be limited due to the size, we will either need to be focused on which features we use or which subset of data we use. Using a system such as dummy variables would not be feasible with the "name" category, so we will need to employ other methods for textual analysis that we are still learning.

### What new technical skills will need to learn in order to complete your project?
To complete this project, we will need to have a thorough understanding of feature selection and have to research into what current trends are used in the development of gaming apps because we want to select the most relevant features in the data set and avoid over-fitting when creating an appropriate model that predicts successful gaming applications. Feature engineering will be performed with machine learning and data manipulation skills we haven't used extensively such as using Variance Threshold or SelectKBest to determine which features are the most important to our analysis.

### How will you conduct your analysis? Please include a detailed description of your intended modeling approach. 

We plan to look at which features in the dataset are most correlated with downloads and also use feature selection to find the most optimal variables to use. We'll then be using predictive modeling using the chosen variables so we'll be able to predict which apps will be most popular. Depending on which machine learning method we use, we may limit our chosen features to a certain amount or compare how well the model performs based on the number of features we feed it.

While initial regressions using OLS will most be cursory, it will give us ideas on which features to include in our machine learning analysis. As well as provide a backdoor into the types of decisions our unsupervised methods. So as stated above, we will be testing different algorithms for polynomial regression, k-means, decision trees, principal component analysis, and support vector machines. These are the methods we have found that may be useful for our categorical features. But determining the best hyper parameters to use will be done with GridSearchCV, and any scalers we use, such as MinMaxScaler for the prices, will be implemented after some basic testing without scalers. 

We will then use plotting methods from pandas and SNS to visualize our results. 

### What major challenges do you anticipate? 

As of now, the major challenges we anticipate are just how we will handle data management. Because of the size, we should be able to drop any rows with null values without any adverse effects. Other than that, choosing the best machine learning method and way to visualize our results may be the most challenging aspect of the project.

We also anticipate challenges learning the best ways to divide textual data, how we can analyse text when there are so many possible combinations of words, and presumably so many frivoulous words that don't indicate something unique about the app, such as "the". Learning the proper machine learning approaches for textual analysis and which are most effective will be a major challenge.