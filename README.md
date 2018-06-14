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
 
 model.predict(predict_col)
 
 
 # Pandas input
 
 def pandas_input(df):
 return tf.estimator.inputs.pandas_input_fn(
 x=df,
 y=df['price'],
 batch_size=128,
 num_epichs=10,
 shuffle=True)
 model.train(pandas_input,steps=2000) 
 
 # Numpy input
  def numpy_input(sqft,prop_type,price):
 return tf.estimator.inputs.numpy_input_fn(
  x={"sq_foot":sqft,"type":prop_type},
 y=price,
 batch_size=128,
 num_epichs=10,
 shuffle=True)
 
