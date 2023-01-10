#Signature_Recognition
capsule network to detect the authentication of a signature

#System requirements
Python 3
Numpy 1.14.6
Tensorflow 1.12.0
Sklearn 0.18.1
Matplotlib 2.1.2
Opencv 3.4.4
Imutils 0.5.1
Keras 2.2.4
PIL 4.0.0

#Dataset
Dataset - This folder contains the genuine images of 12 users. 10per each. which is used for training the model. These images are similar to the drive link shared by the Axis Bank AI Challenge Competetion but few ids are corrected and modified as they were wrong previously. We highly recommend you to use these datasets only as you may find the Ids issues on drive link shared on Hackerearth page which was recokned as false by most of the participants. (check the discussion page for full proof)

TestDriveData1 - Contains 10 Genuine signatures of 5 users for testing. (2 images per user)

TestDriveData2 - Contains 10 Forged signatures of 5 users for testing. (2 images per user)

The capsnet.ipnyb contains the code which is to runned. On running the code , a separate folder called as the output folder will be created and in this folder the checkpoints and other tensorboard requirements will be stored and updated. The checkpoints are loaded during the test time for loading the pre-trained variables.

#Running the code
One can simply open the ipython notebook. Its is suggestible to use the free GPU and TPU provided by google - Google Colaboratory. Since the model consist of multiplication of rank 4 matrices, it would be suggestible to use a GPU if thr code is run on a local computer.

#About the model
For image recognition , traditionally various flavors of CNN were used , but the recent developments bought by Geoffery Hinton , by his state of the art work in Capsule Network seemed to be more promising in the field of computer vision.
The complexity of the model is very high , both in terms of time and memory
