# Data-Science-Interview-Preparation-Series [Github](https://github.com/sunnysavita10/Data-Science-Interview-Prepration/tree/main)

## Day 1 Python Interview Questions [Video]()

* Data Science / ML / DL / GenAI
> Python
>
> Statistics
> 
> Machine Learning
>
> Deep Learning: NLP & CV
>
> Generative AI

* Python
> Condition
>
> Loops
>
> OOPs
>
> exception handling 
>
> file handling
>
> Data stucture (in Python)
> > List
> > 
> > Tuples
> > 
> > Dict
> > 
> > String
> >
>  Function
> > ---
> > Optimization
> >
> > Memory management
> >
> > Design pattern
> > 
> > Scalable

* Statistics
> Descriptive (Data 樣態)
> 
> Inferential (Do testing -- hypothesis testing)

* Machine Learning --> Project (MLOPs) : 類似於 WebDev --> DevOps
> Pipeline (Data ingestion, **Process** (feature engineering), Model, Evaluation (loss/optimization) )
>
> Model building ： hyperparameter tuning
> > Linear regression
> > 
> > Logistic regression
> > 
> > SVM
> > 
> > Decision Tree
> > 
> > Naive bayes
> > 
> > KNN
> > 
> > Random Forest
> > 
> > XGBoost, Gradient Boost, CatBoost, AdaBoost 
> > 
> > Stacking, Boosting, Bagging

* More details about **pipleline** in ML
> Ensemble
>
> Optimization
>
> Loss
>
> Data leakage
>
> Data drift
>
> Cross validation
>
> Feature Engineeging techniques
>
> Dimension reduction
>
> Hyperparameter

* Deep Learning
> ANN
>
> CNN -- CV
>
> RNN -- NLP
>
> Reinforcement Learning
>
> GANs

* Generative AI 
> |LLM/LIM| 
> > text ---->|LLM/LIM|----> text 
> > 
> > image ---->|LLM/LIM|----> text 
> >
> > text ---->|LLM/LIM|----> image 
> > 
> > image ---->|LLM/LIM|----> image 
> |LLM/LIM| : **transformer** can do
> > CV
> > > Detection
> > > 
> > > Segmentation
> 
> RNN --> LSTM/GRU --> Attention (Encoder-Decoder) --> Self-Attention (transformer)
>> transformers --> language translation

* Summary
> Python : 20 ~ 25 quesitons
> 
> Statistics
> 
> ML / ML Project
>
> DL --> ANN, CNN, RNN, LSTM
>
> GenAI --> theory, Practical

## Day 2 Python Interview Questions [Video](https://www.youtube.com/watch?v=OwS9PdbCn1g)
> [Lecture2.ipynb]()

## Day 3 Statistics Interview Questions [Video]()

* Central tendency
> mean
> 
> median
>
> mode

* Data dispersion
> standard deviation
>
> variance

* Data distribution - PMF & PDF
> continuous variable
>
> discret variable

* Probability theory

* Population / Sampling

* Inferential statistics (hypothesis testing)

** Point estimate

** confidence interval

** p-value

** Significace level

** Standard error

** One / Two tail test

** Z-test / t-test / chi-square

** anova test

## Day 4

* [Significant Level -- Critial Interval](https://wbd.ms/share/v2/aHR0cHM6Ly93aGl0ZWJvYXJkLm1pY3Jvc29mdC5jb20vYXBpL3YxLjAvd2hpdGVib2FyZHMvcmVkZWVtL2M5MGM1YmUyMWE5ZDQ2NzFhYjkxYWRkMzE1NGE5NTYyX0JCQTcxNzYyLTEyRTAtNDJFMS1CMzI0LTVCMTMxRjQyNEUzRF82MzQ1Y2E2NS0wYjg1LTRhMzEtYmIxOC1mYzc5NTY3NGM5ODk=)

* [Confidence Intervals, Margins of Error, and Confidence Levels](https://www.nngroup.com/articles/confidence-interval/)

* [Ways to get a more precise confidence interval](https://support.minitab.com/en-us/minitab/help-and-how-to/statistics/basic-statistics/supporting-topics/basics/ways-to-get-a-more-precise-confidence-interval/) 

## Day 5 Machine Learning Interview Questions Part 2 [Video](https://www.youtube.com/watch?v=DB4UTf96xa4)
* The pipeline of Machine Learning:
> > (Stream, Batch, Mini batch)
>
> 1. Data ingestion
>
> 2. Data validation
>
> 3. EDA -- Explore Data Analysis
>
> 4. Preprocessing (feature engineering)
>
> 5. Model building
> > supervised vs. unsupervised
>
> 6. Model evaluation
> > Supervised: Regression, Classification
> >
> > Unsupervised: Clustering
>
> 7. Deploy
>
> 8. Monitor
> 
> 9. Maintainance
>
> 10. Retraining

* Q1. The distinction between parametric and non-parametric algorithms liesin how they make assumptions about the underlying data distribution.
> **parametric**
> > Complex data (X)
> > 
> > Regression -- y = mx + c (function)
>
> **non-parametric**
> > Complex data (O)
> >
> > Decision tree -- condition determination 

* Q2. Difference between convex and non-convex cost function; what does it mean when a cost function is non-convex?

The distinction between convex and non-convex cost functions is important in
optimization problems, particularly in the context of machine learning and
deep learning.

Supervised ML 
> Training (Linear regression -- y = mx + c)
> > 1. Calculation
> >
> > 2. Loss calculation
> >
> > 3. optimization (derivative of loss)
> > > Gradient descent (GD)
> > > > SGD
> > > > 
> > > >  Minibatch
> > 

MSE in terms of machine learning is going to behave as a convex function.

And the same function -- MSE -- itself in the Deep learning with respect to the artificial neural network
it's going to behave as a non-convex method.

* Q3. Give me an example of when False positive is more crucial than false negative and vice versa give me an example.
Model Evaluation --> classification

Confusion Matrix --> 2 classes

P (Prediction), A (Actual)
P\A |  0  |  1  
-- -- -- -- -- -- 
1   |  FP |  TP
-- -- -- -- -- -- 
0   |  TN |  FN

FP -->  Type I error --> A: negative | P: positive

FN --> Type II error --> A: positive | P: negative

Domain
> Health care (e.g., Heart disease) 
> > FN 是嚴重的問題
> Stock price 
> > FN 會損是金錢，預測不會下跌，但卻下跌 (crash)
> Spam 
> > FP 會是嚴重的，若正常郵件被預測為 spam，但事實上不是 spam，則錯過來自郵件重大事情



* Q4. Why KNN is known as a lazy learning technique?

Data 準備好時
> * Training -- 3 steps
> > Calculation
> 
> > Loss Calculation
> 
> > Optimization
> * Prediction
> >

KNN is a lazy learning, because we don't have any sort of a learning over here.
This is a data mining technique.
然而 KNN 在 training 時，不需要用到 3 steps，而是直接算出 distance 後 分群


* Q5. What do you mean by semi-supervised learning?
ML
> Supervised
> > Independent Columns --(預測)--> Dependent value
>
> Unsupervised
> > (training) 獲得 Similar pattern -- group
> > 
> > (test) evaluation
> 
> Semi-supervised
> 先 group (unsupervised)，再 分類 (supervised)

* Q6 What is an OOB (out of bag instances) error and how is it useful?

RF (random forest) -- Bootstrap + Aggregation
> Bootstrap
> > | C + R | --> 分類 TREE

C 是 column -- 從 Data 中 選取 feature

R 是 row -- 從 Data 中 選取一筆筆的 資料 

好處
> Easily monitor the performance of the model
> 
> Separate validation is not required, so we can save that effort over here.
We are going to do a validation and we just do on the random data set.
Which means our model don't know which data set will come every time basically 
it will get the random data set.

* Q7. In what scenario decision tree should be preferred over random forest?

Decision tree 容易造成 overfitting 的問題，random forest 優點就是提供了一個 generalized model.

1. explain

2. computation

3. feature

[參考](https://www.youtube.com/watch?v=1pIrDi6puGs)

* Q8. Imagine you are working with a laptop of 2GB RAM, how would you process a dataset of 10 GB?

兩個考量點 -- M , P
> M : memory
>
> P : processing (計算或處理能力)

1. chunk

2. Streaming (different system/way)

3. Parallel processing (M+P)

4. Sample (mathematics)

5. Database (separate concept)

6. Distributed (M+P)

7. Dimension reduce (mathematical one)

8. Incremental learning (training the model into the multiple stages)

## Day 6 Deep Learning Interview Questions [Video](https://www.youtube.com/watch?v=btWwUla9oJ8)

* Q1. What are the main differences between Structured and Unstructured Data?

Structured
> tabular

Unstructured
> Image
>
> Video
>
> Text
>
> Audio

* Q2. What are the main points of difference between Bagging and Boosting?

Ensemble -- group of models
> Bagging (Parallel fashion -- create multiple models all together) 
> > Boostrap -- a way of collecting the samples 
> > > Sampling (R+C) -- 例如 Random Forest
> >
> > Aggregation (taking majority count)
>
> Boosting -- chain of the model
> > XGBoost, Gradient Boost [圖形筆記](https://wbd.ms/share/v2/aHR0cHM6Ly93aGl0ZWJvYXJkLm1pY3Jvc29mdC5jb20vYXBpL3YxLjAvd2hpdGVib2FyZHMvcmVkZWVtL2U2ZjE2ODBiZWEyZDQwMzlhMTA3MTYyNDE1ZjFiYjk0X0JCQTcxNzYyLTEyRTAtNDJFMS1CMzI0LTVCMTMxRjQyNEUzRF85YzY3OTlhOS1mODQ4LTRiNGMtYjVhNi1lNmFiYjQ3YTQ5MTU=)
>
> Stacking

注意:Bagging 不算是 Algorithm 而是一種 Way/Method, Bagging 與 Boosting都是 homogeneous, Stacking 則是 hetrogeneous

補充問題：What is the difference between random forest and the bagging classifier

Hint:
> In the bagging classifier if we are taking the decision tree, it's similar to the random forest.

參見: 
> [BaggingClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.BaggingClassifier.html)
> > 用 Homogeneous: At a time we can take only single algorithm 
> [RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)


Simple answer:
> In bagging, weak learners are trained in parallel, but in boosting, they learn sequentially (a sequence of weak learners).

補充點：Stacking [提升準確度的最後一哩路：stacking](https://celiachen01.wordpress.com/2022/01/31/%E6%8F%90%E5%8D%87%E6%BA%96%E7%A2%BA%E5%BA%A6%E7%9A%84%E6%9C%80%E5%BE%8C%E4%B8%80%E5%93%A9%E8%B7%AF%EF%BC%9Astacking/)
> training
>
> meta training

[補充參考](https://tomohiroliu22.medium.com/985c5b09546f)

* Q3. What are the assumptions of linear regression?

[Solution](https://www.geeksforgeeks.org/assumptions-of-linear-regression/)

* Q3-1. Why logistic regression is called Regression?

Because there also we are using that particular line and it's nothing this logistic regression
it's a transformation of that line itself.

* Q4. How do you measure the accuracy of a Clustering Algorithm?

`Clustering` is called group ing of the data. We have `Silhouette Score`, `wcss values`, `done index`, `jagat similarity`.

[參考答案](https://analytical.quora.com/How-to-measure-the-accuracy-of-a-clustering-Algorithm)

* Q5. What is an imbalanced Dataset and how can one deal with this problem?

注意，`imbalanced` means that we have the ratio of the classes will be different

參考：[imbalanced-learn documentation](https://imbalanced-learn.org/stable/user_guide.html#user-guide)

* Q6. What is Data Leakage? List some ways using which you can overcome this problem.

在 preprocessing data 時，會執行 deal with outliers, missing values, perform the scaling of the data, perform the encoding. 但在preprocessing 之前，還有一個步驟，就是把 data 分成 training set, validation set, 和 test set.

參考答案：During training, test data is known.

* Q7. What is multicollinearity? How to detect it? List some techniques to overcome multicollinearity.

`multicollinearity` means the correlation between two columns and correlation with target column.

Highly correlation among the features. So if we are taking only single feature in that case. 
Also, we can find out the good pattern from the pattern from the data itself.

To detect the multicolinearity, you can design the correlation Matrix.
1. Calculate Corr
2. Calculate VIF: 計算 R-squared value

* Q8. List some ways using which you can reduce overfitting in a model.

overfitting: train時，performance好，test時，performance差

underfitted: 以上兩個過程，performance都變差

可以用 cross-validation, 收集more data, 用不同 preprocessing technique (feature selection, PCS, reduce dimension) 

[參考](https://aws.amazon.com/what-is/overfitting/)

* Q9. How do you approach a categorical feature with high cardinality?

high cardinality: huge number of unique values

1. frequency based encoding

2. target encoding

~. one hot encoding with frequency threshold

3. Binary encoding

4. Dimension reduction (if having sparse matrix) (embedding)

[參考(Data Science Interview Questions from Giants)](https://yoyoinwanderland.github.io/2017/04/06/Data-Science-Interview-Questions-from-Giants/)

* Q10. Explain neural network in terms of mathematical function.
Can I solve problem of classification with tabular data in neural network?

1. Weight

2. Bias

3. Activation

4. Loss

5. Optimizer

6. Normalization

7. Drop-off

8. Number of parameters
 
9. Epoch (one back propagation) 

10. Nodes & edges (hyperparameter)

Output = Act(x1w1+x2w2+x3w3+...+b)

* Q11. Can you please explain difference between sigmoid & tanh function.
What is learning rate in laymaen way and how do you control learning rate?

[Solution (Most asked ML and DL Interview Questions Set 2(75 to 85))](https://manojprabakarann.medium.com/82364f7b7e65)

## Day 7 Generative AI Interview Questions [Video]()

1. ANN

2. CNN --> Computer Vision

3. RNN --> NL --> Generative AI (LLM)

4. RL


* Topics of `Artificial Neural Network` here
> 1. Introduction of NN (DL)
>
> 2. Perceptron
> 
> 3. Activation
>
> 4. Loss function
>
> 5. Backpropogation(optimizer)
> 
> 6. Callbacks
>
> 7. Early stopping 
>
> 8. Regularization
> 
> 9. Normzlization
>
> 10. Weight initialization
>
> 11. Hyperparameter tuning

ML VS. DL
> 1. Data (tabular data vs. unstructured data)
>
> 2. training time
>
> 3. hardware dependency (it is there with respect to DL. it's not there in ML)
>
> 4. feature extraction/ feature selection (it automatically extracts features with respect to DL. Manually in ML)
> 
> 5. interpretability (it is little hard in DL)

How to improve the performance in DL
> 1. Hyperparameter tuning (nodes, layers, epoches)
>
> 2. Optimizer
>
> 3. Regularization (L1, L2)
>
> 4. Normalization
>
> 5. Weight initialization
>
> 6. Early stopping
>
> 7. Batch size


[Keras all CNN Architecture -- Keras Applications](https://keras.io/api/applications/)
> based on the changes in the kernels, based on the changes in the number of features

* `Inception Network` 
> [介紹 Inception network ](https://ithelp.ithome.com.tw/m/articles/10205210)

Convolution is the fundamental unit of the computer vision.

* Vision Transformer (ViT)

[CNN_Architecture](https://wbd.ms/share/v2/aHR0cHM6Ly93aGl0ZWJvYXJkLm1pY3Jvc29mdC5jb20vYXBpL3YxLjAvd2hpdGVib2FyZHMvcmVkZWVtLzAzMTE3MDQxYmFmMjRiOWVhMDRiMjdlNWFhYmY0NTc5X0JCQTcxNzYyLTEyRTAtNDJFMS1CMzI0LTVCMTMxRjQyNEUzRF9jMzEwZDk3Mi01N2UxLTQxMmEtODM0OC00MGMxMTAxMWE2MDg=)

* In the classical machine learning and deep learnin 

1. Discriminative process

(training stage)
> 1. Data ingestion (collection)
>
> 2. Analysis on top of it
>
> 3. Preprocessing
>
> 4. Model creation
>
> 5. Evaluation
>

(prediction state) 
> feature (data) --> |Model| --> output
                      ^^^^^ (use case specific)

discriminative cases (classification)
> Cancer VS. not cancer
>
> Diabetes VS. not diabetes

2. Generative Model (LLM -- Large Language Model)

(training -- Unsupervised LM --> Supervised fine tuning)
> 1. Data -- huge
>
> 2. Analysis
>
> 3. Preprocess
>
> 4. Model -- generalization (非 use case)
> > LLM --> transformer (NN + Self-Attention)
>
> 5. Evaluation

(inferencing -- prediction)
> prompt --> |Model| --> generate

## Day 8 Resume Building Data science [Video](https://www.youtube.com/watch?v=HN2jlmVq8_I)

* GENAI
> 1. NLP (Encoder & Decoder)
>
> 2. Attention
>
> 3. Transformer (Self Attention) (Encoder & Decoder)
> 
> 4. BERT (Encoder)
> 
> 5. GPT (Decoder)

* Language task
> 1. text classification
> 
> 2. text summarization
>
> 3. text generation
>
> 4. Question/Answer/Chatbot

* Langchain / Llama-index
> API / Finetuning / RAG