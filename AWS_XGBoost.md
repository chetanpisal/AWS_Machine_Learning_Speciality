## AWS XGBoost


The XGBoost (eXtreme Gradient Boosting) is a popular and efficient open-source implementation of the gradient boosted trees algorithm. Gradient boosting is a supervised learning algorithm that attempts to accurately predict a target variable by combining an ensemble of estimates from a set of simpler and weaker models. The XGBoost algorithm performs well in machine learning competitions because of its robust handling of a variety of data types, relationships, distributions, and the variety of hyperparameters that you can fine-tune. You can use XGBoost for regression, classification (binary and multiclass), and ranking problems.

You can use the new release of the XGBoost algorithm either as a Amazon SageMaker built-in algorithm or as a framework to run training scripts in your local environments. This implementation has a smaller memory footprint, better logging, improved hyperparameter validation, and an expanded set of metrics than the original versions. It provides an XGBoost estimator that executes a training script in a managed XGBoost environment. The current release of SageMaker XGBoost is based on the original XGBoost versions 0.90 and 1.0.


**XGBoost Algorithm**_Type:_. {SUPERVISED} 
• eXtreme Gradient Boosting• Gradient boosted trees algorithm_Use cases:_• Making predictions from tabular data


XGBoostOpen-source implementation of the gradient boosted trees algorithm that attempts to accurately predict a target variable by combining the estimates of a set of simpler, weaker models.A virtual “Swiss army knife” for all sorts of regression,classification and ranking problems, with 2 required and 35 optional hyperparameters to tune.Accepts CSV and libsvm for training and inference 

Uses tabular data with rows representingobservations, one column representing the target variable or label and the remainingcolumns representing features.Only trains on CPU and memory bound.Currently only trains on CPU instances and is memory-bound as opposed to computebound.Recommend lots of memory.AWS recommends using an instance with enough memory to hold the entire trainingdata for optimal performance. 

Spark IntegrationUsing the SageMaker Spark SDK, you can call XGBoost direct from within the Spark environment.


### XGBoost Use cases• RankingExample: On an e-commerce website, you can leverage data about search results, clicks,and successful purchases, and then use XGBoost to train a model that can returnrelevance scores for searched products.
• Fraud DetectionExample: When XGBoost is given a dataset of past transactions and whether or not theywere fraudulent, it can learn a function that maps input transaction data to the probabilitythat transaction was fraudulent.