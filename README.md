# IDS by siamese neural network


This project demonstrates the ability of siamese neural networks to detect malicious network packets.

# NSL-KDD Dataset
The NSL-KDD dataset consists of a total of 39 network attack packets.
![캡처](https://user-images.githubusercontent.com/42932423/104112300-86cc3e80-5330-11eb-9ab8-7af573a17397.PNG)

The number of training data is as follows
![캡처](https://user-images.githubusercontent.com/42932423/104112341-03f7b380-5331-11eb-9036-ce9e234e9fe6.PNG)

The number of test data is as follows
![캡처](https://user-images.githubusercontent.com/42932423/104112390-95ffbc00-5331-11eb-85fb-84e96aacbf71.PNG)

# Preprocessing
  - First, normalization of NSL-KDD data was performed.
  - Second, to balance the unbalanced data, oversampling was performed for each label.
  - Third, we created true data paired with data within the same label, and created false data paired with other labels.
![캡처](https://user-images.githubusercontent.com/42932423/104112438-30f89600-5332-11eb-8eec-cc763062d30d.PNG)

# Neural network model
![캡처](https://user-images.githubusercontent.com/42932423/104112227-78315780-532f-11eb-9415-c55d9a0086b8.PNG)

# Result
We evaluated one-shot n-way learning with some data. The accuracy according to the value of n is as follows.
![캡처](https://user-images.githubusercontent.com/42932423/104112584-e841dc80-5333-11eb-965e-c4b632ad8d57.PNG)
