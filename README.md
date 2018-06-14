# GCP-TF

1. features_col =[tf.feature_column.numeric_column("sq_footage"),tf.feature_column.categorical_column_with_vocab_list("type),["house","apt"]]

model=tf.estimator.LinearRegressor(features_col,''./model_training')

def train_col():
 features={"sq_foot":[100,200,400],"type":["house","apt","apt"]}
 labels=[]
 return freatures, labels
 
 model.train(train_col,steps=2000)
 
 def predict_col():
 features= {}
 return features
 
 model.preduct(predict_col)
 
