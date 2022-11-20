# Module_14_Challenge: Machine Learning Trading Bot
In this Challenge, we are assuming the role of a financial advisor at one of the top five financial advisory firms in the world. Our firm constantly competes with the other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, your firm has heavily profited by using computer algorithms that can buy and sell faster than human traders.

The speed of these transactions gave your firm a competitive advantage early on. But, people still need to specifically program these systems, which limits their ability to adapt to new data. You’re thus planning to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market. To do so, we will  enhance the existing trading signals with machine learning algorithms that can adapt to new data.

We were requested to divide the challenge into the following sections:

- Establish a Baseline Performance

- Tune the Baseline Trading Algorithm

- Evaluate a New Machine Learning Classifier

- Create an Evaluation Report


The initial analysis we looked at using short and long window SMA values of 4 and 100.  The following results are displayed.

<img width="543" alt="Screen Shot_1_Baseline_Cumulative_return_plot" src="https://user-images.githubusercontent.com/108632632/202889641-d93789da-8f05-4c88-a05c-fd8069fa7d65.png">

<img width="744" alt="Screen Shot_2__Baseline_ 2022-11-20 at 11 10 46 am" src="https://user-images.githubusercontent.com/108632632/202889649-292a3f2f-9501-4c1e-a3ab-6a2ccb574aea.png">

<img width="622" alt="Screen Shot_3_baseline" src="https://user-images.githubusercontent.com/108632632/202889669-c1d225c3-1389-4518-afe3-001136d430c4.png">

The data was then split and we used the SVC classifier model from SKLearn to fit the training data and make some predicitions.

<img width="560" alt="Screen Shot_7__SVC_predictions_ 2022-11-20 at 5 50 35 pm" src="https://user-images.githubusercontent.com/108632632/202889811-947e35f3-df0d-49d2-8a0f-1d44dcef6741.png">

A new classifier Logistic Regression was used to backtest the model.

<img width="697" alt="Screen Shot_6_New_classifier_and_backtest_ 2022-11-20 at 11 18 34 am" src="https://user-images.githubusercontent.com/108632632/202889979-7cb59436-e59b-4ff2-9d37-ce46c4b154fe.png">

<img width="671" alt="Screen Shot_4" src="https://user-images.githubusercontent.com/108632632/202889997-b036dc48-e674-48c7-8cc3-e0d2e73ece8e.png">

The following results are displayed when we increased the short and long window SMA values to 50 and 100. 

<img width="572" alt="Screen Shot 2022-11-20 at 6 04 28 pm" src="https://user-images.githubusercontent.com/108632632/202890150-e4e1b86c-fd53-49d2-a498-ab86068d66b2.png">

<img width="650" alt="Screen Shot 2022-11-20 at 6 06 22 pm" src="https://user-images.githubusercontent.com/108632632/202890211-c1eb4f98-4f6d-49d6-9077-d7b2b05e9a20.png">

<img width="803" alt="Screen Shot _10_2022-11-20 at 6 07 50 pm" src="https://user-images.githubusercontent.com/108632632/202890256-b3a083dc-e0eb-49d9-a0f2-fcf159db7373.png">

 A minimal insignificant change was reflected when changing the windows.  

**Technologies used:**

- Pandas

- Numpy

- Hvplot

- Scikit-learn

