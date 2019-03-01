# INFO 370 Final Project
## Project Description
### What is the overarching purpose of your research project, and why is it an important undertaking?
There are many apps currently on the market. While some applications are popular, others are not. We wanted to determine what factors play a role on an application’s popularity and thus predict an applications popularity based upon it. This task is important as it allows developers and companies to determine the best possible application to create in order to create a widely used application. Our findings will even the playing field for companies/enterpreneurs attempting to break into the mobile gaming industry by providing knowledge of what makes a successful application, as well as provide students interested in the gaming industry with an understanding of what makes an app popular. Furthermore, we are helping users of gaming apps because by openly sharing what makes a gaming app competitive in an open market, companies will pick up on this and users will have a more competitive market of gaming apps to choose from. 

### How does your research fit into the broader problem domain? You should cite at least 3 papers that help contextualize your research. 

The broader problem domain is determining the probaility of an application making a profit. Our research focuses on whether an application will be popular because if we can determine whether an application will be popular, there will be a greater chance of it making a profit for the developers/companies, and in return, we create business knowledge that is helpful for the gaming industry as a whole. From our careful research we have learned that applications who have more recent updates tend to be more popular as well as target demographics having a greater impact on the popularity. We also gained insight that certain app rating affects the popularity of the app, as it targets different audiences. Technologies used also has an influence on the popularity of an app, as visual stimulation and fast-rendering is directly related to the technologies used to create the app.  Through the research we may be able to determine for example: maturity-rating may be one of the most important factors and what rating one should aim for to make a successful application.

Sources:
* https://arxiv.org/pdf/1802.02996.pdf
* https://arxiv.org/pdf/1603.00059.pdf
* http://www.pewinternet.org/2015/11/10/an-analysis-of-apps-in-the-google-play-store/
* https://www.newgenapps.com/blog/steps-successful-mobile-game-development

### What specific hypothesis (hypotheses) are you going to test?
If a developer/company follows the current trends, creating an application with similar features as the most popular apps, then the app will have more installs, because it appeals to a broader audience.

### What are the datasets you'll be working with to answer this question? Please include relevant background describing the datasets you identify.
The dataset we will be working with in this research project was web scraped by a user on Kaggle at:
* https://www.kaggle.com/lava18/google-play-store-apps
The dataset holds information such as maturity-rating, payment-model, applications size, etc.

### What statistical and machine learning methods do you plan on using to test your hypothesis?
We plan to use a few methods, some of which are: multiple linear regressions, univariate analysis and bivariate analysis.

### Who is your target audience for the resource you will build? Depending on the domain of your data, there may be a variety of audiences interested in using the dataset. You should hone in on one of these audiences.
The target audience in the our research projects would be individual developers / companies as they want to create an application with the best chance of mainstream success.

### What should your audience learn from your resource? Consider specific questions they may want to answer.
The audience would learn from the resource is: “what type of application would be best to create”. That is based upon the application’s pay-model, genre, maturity rating, etc; we wanted to determine which factors the most into an application’s success. Or  “will making my application pay-to-use decrease it’s popularity?” 

## Technical Description
### What will be the format of your final web resource (Shiny app, HTML page or slideshow compiled with KnitR, etc.)?
A Jupyter Notebook created report (Maybe?)
### Do you anticipate any specific data collection / data management challenges?
There may be duplicate entries for the same application, we’re going to need to clean this up if that is the case. The dataset is pretty huge, this may cause technical issues, we might need to run our analysis on a third of the dataset as opposed to the whole dataset at any given time.

### What new technical skills will need to learn in order to complete your project?
To complete this project, we will need to have a thorough understanding of feature selection and have to research into what current trends are used in the development of gaming apps because we want to select the most relevant features in the data set and avoid over-fitting when creating an appropriate model that predicts successful gaming applications

We will also need to understand different machine learning technologies that are able to use historical data to predict the success of an application. We currently understand grid search from lecture, but is this the best method to use for our data? This is a question we will need to answer by learning what machine learning models are available to us. 
### How will you conduct your analysis? Please include a detailed description of your intended modeling approach. 

### What major challenges do you anticipate? 

