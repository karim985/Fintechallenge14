
## Machine Learning Trading Bot¶


Our firm competes with other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, our firm has profited heavily by using computer algorithms that can buy and sell faster than human traders.
We plan to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market. To do so, you’ll enhance the existing trading signals with machine learning algorithms that can adapt to new data.
We will combine algorithmic trading, financial Python programming, and machine learning to create an algorithmic trading bot that learns and adapts to new data and evolving markets.

## Project road map:

Establishing a Baseline Performance

Tuning  the Baseline Trading Algorithm

Evaluating a New Machine Learning Classifier

Creating an Evaluation Report

**Establish a Baseline Performance**

![Image 01](http://localhost:8888/files/Desktop/Fintechallenge14/images%20/image01.png?_xsrf=2%7Cb57baf9f%7C02c30d444ee3be73843f61fb00843037%7C1673288267)

![Image 02](http://localhost:8888/files/Desktop/Fintechallenge14/images%20/image02.png?_xsrf=2%7Cb57baf9f%7C02c30d444ee3be73843f61fb00843037%7C1673288267)

The baseline performence has an accuracy of 55%, and that's by Using the `SVC` classifier model from `SKLearn's` support vector machine (SVM) learning method.
Generating trading signals using short window(4)- and long-window(100) SMA values.
this model would perfomed butter if predicted more negative returns 



**modifing SMA short window to 2**
![image 05](http://localhost:8888/files/Desktop/Fintechallenge14/images%20/image05.png?_xsrf=2%7Cb57baf9f%7C02c30d444ee3be73843f61fb00843037%7C1673288267)

![image 06](http://localhost:8888/files/Desktop/Fintechallenge14/images%20/image06.png?_xsrf=2%7Cb57baf9f%7C02c30d444ee3be73843f61fb00843037%7C1673288267)
Decreasing SMA window to 2 made slight changes on the accuracy and precision but big impact on recall where this model got a lot of negativies return (78%) and less incorrect negativies return
this model did better on predicting the negative class 
**adjusting the size of the training dataset to 6 months**


![image 03](http://localhost:8888/files/Desktop/Fintechallenge14/images%20/image03.png?_xsrf=2%7Cb57baf9f%7C02c30d444ee3be73843f61fb00843037%7C1673288267)

![image 04](http://localhost:8888/files/Desktop/Fintechallenge14/images%20/image04.png?_xsrf=2%7Cb57baf9f%7C02c30d444ee3be73843f61fb00843037%7C1673288267)

adjusting the size of the training dataset to 6 months made some improvement on accuaracy compared to the baseline model 

**Evaluate a New Machine Learning Classifier**

In this section, we will use the original parameters that the starter code provided. But, we will apply them to the performance of a second machine learning model `DecisionTreeClassifier`

`DecisionTreeClassifier`is a class capable of performing multi-class classification on a dataset. In case that there are multiple classes with the same and highest probability, the classifier will predict the class with the lowest index amongst those classes.

![image 07](http://localhost:8888/files/Desktop/Fintechallenge14/images%20/image07.png?_xsrf=2%7Cb57baf9f%7C02c30d444ee3be73843f61fb00843037%7C1673288267)

![image 08](http://localhost:8888/files/Desktop/Fintechallenge14/images%20/image08.png?_xsrf=2%7Cb57baf9f%7C02c30d444ee3be73843f61fb00843037%7C1673288267)
the new ML classifier gave us good precion but was more efficient on predicting the (-1) class 

**Summary**

We can definitly say that adjusting the size of the training dataset to 6 months improved the accuracy, recall and f1 score of the class(1) there for we will keep this model. 


## Contributer

[Karim Bouzina](https://www.linkedin.com/in/karim-bouzina-574348244/)

## Licence 

© 2023 edX Boot Camps LLC

     UW Fintech 


