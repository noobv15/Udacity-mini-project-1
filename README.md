# Udacity-mini-project-1
#Naive Bayes
from sklearn.naive_bayes import GaussianNB
from sklearn.metrics import accuracy_score
clf=GaussianNB()
clf.fit(features_train,label_train)
pred=clf.predict(features_test)
accuracy = accuracy_score(pred,label_test)
print("Accuracy is : " + accuracy)
