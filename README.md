# Text-Classification-with-kNN
Develop predictive models that can determine, given a medical abstract, which of 5 classes it falls in.


Medical abstracts describe the current conditions of a patient. Doctors routinely scan dozens or hundreds of abstracts each day as they do their rounds in a hospital and must quickly pick up on the salient information pointing to the patient’s malady. The goal is to design assistive technology that can identify, with high precision, the class of problems described in the abstract. In the given dataset, abstracts from 5 different conditions have been included: digestive system diseases, cardiovascular diseases, neoplasms, nervous system diseases, and general pathological conditions.

The purpose of this competition is to allow me to develop predictive models that can determine, given a particular medical abstract, which one of 5 classes it belongs to. As such, the goal would be to develop the best classification model, with the restriction that you can only use your own implementation of the min-epsilon k-NN classifier.

The min-epsilon k-NN classifier is defined similarly as the k-NN classifier with the exception that neighbors 2 to k are additionally restricted to have a minimum similarity of epsilon with the query object. In other words, restrict neighbors by both number of neighbors and minimum similarity, but always retrieve at least one neighbor. Given the retrieved neighbors, I still have to decide on the way you aggregate their labels to make the final decision (e.g., majority count or weighted sum). Working with distances instead of similarities works as well, only needs change the problem into a max-epsilon k-NN problem, where epsilon is the maximum distance from the query.



Data Description:

The training dataset consists of 14438 records and the test dataset consists of 14442 records. Training class labels are provided and the test labels are held out. The data are provided as text in train.dat and test.dat, which should be processed appropriately.

train.dat: Training set (class label, followed by a tab separating character and the text of the medical abstract).

test.dat: Testing set (text of medical abstracts in lines, no class label provided). 

format.dat: A sample submission with 14442 entries randomly chosen to be 1 to 5.
