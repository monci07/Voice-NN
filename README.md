# Voice-NN
Speach to text NN project

## Summary
The objective of this project is use a NN to recognize a key-word and once it hears it, it will activate the listining part of the program to receive an order.

## Planning
The tecnologies I decided to use are:
* Jupyter notebook to conduct the training of the models.
* For the audio I decided to use pyaudio.
* For the NN will be the Tensorflow API.
* For the final aplication will be scripted in python.  
  
(These technology's are not final and may change in the future)

I divided the project in 5 parts:
1. Create n number of samples to train the NN for recognicing the key-word. The samples are divided in "negatives" and "positives", at the moment im not quite sure how many of each I will need.
2. Experiment with different type of recursive NN structures to be able to predict when the computer recieves the activation word.
3. Ones the previous step is done, its time to create a data-set of words.
4. Here is either two options:
   1. Change the last layer of the previous NN to predict letters and form words.
   2. Use a whole new NN.
5. Put it all together.

I will try to keep every thing explained in these README and in each notebook.

As for now the project its in the third part.

### First part
All the information its  on the jupyter notebook.

### Second part
Right know the structured model makes a prediction of 70-80% accuracy with a 50-60% loss. I will try to make a way to make the numpy arrays into spectograms to get a lower loss at the time of training.

#### **_UPDATE as of 09/26/2022_**
Tried with a spectogram data set for the training, got much less the same result, so i will continue to try a different approach. Got a train loss: 0.5251 and a train accuracy: 0.7880. and on a dev/test got a loss: 0.4785 and accuracy: 0.8150.

#### **_UPDATE as of 10/17/2022_**
Returned to my original idea of using the data almost raw(i just turned the bytes into floats) and make the NN a little deeper, got to see a improvement in the training but a deficit in the dev/test. Got a train loss: 0.5215 and a train accuracy: 0.8080, and on a dev/test got a loss: 0.5194 and accuracy: 0.7980.

#### **_UPDATE as of 10/23/2022_**
Following the last update, and analizing the data better, I started to work on changing the learning rate to see any kind of improvement. After much testing got a perfect lerning rate that got me a train loss of 0.0803 and a accuracy of 0.9705, and a dev/test loss of 0.0337 and a accuracy: 1.0000, I will try using it in a normal python code.

For all the information, it will be in the Jupiter notebook
