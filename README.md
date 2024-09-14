# bank-marketing-by-oumaima-gasmi-
The older marketing options have contributed minimal in increasing the business of banks. Due to internal competition and financial crisis European Banks were under pressure to increase their financial assets. They offered long term deposits with good interest rates to the people using direct marketing strategy but contacting many people takes lot of time and success rate is also less. So they want to take help of the technology to come up with a solution that increases the efficiency by making fewer calls but improves the success rate.Portuguese Banking Institution has provided the data related to marketing campaigns that took over phone calls.  

BUSINESS PROBLEM: Finding out the characteristics that are helping Bank to make customers successfully subscribe for deposits, which helps in increasing campaign efficiently and selecting high value customers.  MACHINE LEARNING PROBLEM: The goal is to build Machine Learning model that learns the unknown patterns, maps and several input features classifying whether client will subscribe for longer deposits or not.  



DATA SET OVERVIEW:  The data is related with direct marketing campaigns of a Portuguese banking institution.The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be (‘yes’) or (‘no’).  The data set is taken from UCI Machine Learning repository: 
1) bank-additional-full.csv with all examples (41188),
2) 2) bank-additional.csv with 10% of the examples (4119).
   3) Attribute Information:  Input variables: # bank client data:
      1 — age (numeric)
      2 — job : type of job (categorical: ‘admin.’,’blue-collar’,’entrepreneur’,’housemaid’,’management’,’retired’,’self-employed’,’services’,’student’,’technician’,’unemployed’,’unknown’)
      3 — marital : marital status (categorical: ‘divorced’, ‘married’, ‘single’, ‘unknown’; note: ‘divorced’ means divorced or widowed)
      4 — education (categorical: ‘basic.4y’,’basic.6y’,’basic.9y’,’high.school’,’illiterate’,’professional.course’,’university.degree’,’unknown’)
      5 — default: has credit in default? (categorical: ‘no’, ‘yes’, ‘unknown’) 6 — housing: has housing loan? (categorical: ‘no’, ‘yes’ ,’unknown’)
      7 — loan: has personal loan? (categorical: ‘no’, ‘yes’, ‘unknown’) # related with the last contact of the current campaign:
      8 — contact: contact communication type (categorical: ‘cellular’, ‘telephone’)
      9 — month: last contact month of year (categorical: ‘jan’, ‘feb’, ‘mar’, …, ‘nov’, ‘dec’)
      10 — day_of_week: last contact day of the week (categorical: ‘mon’,’tue’,’wed’,’thu’,’fri’)
      11 — duration: last contact duration, in seconds (numeric).
      Important note: this attribute highly affects the output target (e.g., if duration=0 then y=’no’). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.  # other attributes:
      12 — campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
      13 — pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)
      14 — previous: number of contacts performed before this campaign and for this client (numeric)
      15 — poutcome: outcome of the previous marketing campaign (categorical: ‘failure’,’nonexistent’,’success’)  # social and economic context attributes
      16 — emp.var.rate: employment variation rate — quarterly indicator (numeric)
      17 — cons.price.idx: consumer price index — monthly indicator (numeric)
      18 — cons.conf.idx: consumer confidence index — monthly indicator (numeric)
      19 — euribor3m: euribor 3 month rate — daily indicator (numeric)
      20 — nr.employed: number of employees — quarterly indicator (numeric)  Output variable (desired target):
      21 — y — has the client subscribed a term deposit? (binary: ‘yes’, ‘no’)
PERFORMANCE METRICS:  Different performance metrics are used to evaluate machine learning model. Based on our task we can choose our performance metrics. Since our task is of classification and that too binary class classification, whether client will or will not subscribe for deposits.  PRIMARY PERFORMANCE METRICS  Here we will be using AUC ROC curve.
What is ROC?  ROC also known as Receiver Operating Characteristics, shows the performance of binary class classifiers across the range of all possible thresholds plotting between true positive rate and 1-false positive rate  What is AUC-ROC?  AUC measures the likelihood of two given random points, one from positive and one from negative, the classifier will rank the positive points above negative points. AUC-ROC is popular classification metric that presents the advantage of being independent of false positive or negative points.
      Ideal AUC-ROC score is 1. AUC-ROC score for random classifier is 0.5.  SECONDARY PERFORMANCE METRICS  Macro-F1 Score: F1 score is the harmonic mean between Precision and Recall.
      Macro F1 score is used to know how our model works in overall dataset.  Confusion Matrix: This matrix gives the count of true negative, true positive, false positive and false negative data points.  EDA:  Before going further let’s understand what is EDA?  EDA is a way of interpreting, summarising and visualizing the dataset's information. It could help us to identify patterns and relationships that may not be understood or visible. It is the one of the important things in data science life cycle.
