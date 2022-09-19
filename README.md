# Voice-NN
Speach to text NN project

## Summary
The objective of this project is use a NN to recognize a key-word and once it hears it, it will activate the listining part of the program to receive an order.

## Planning
The tecnologys I decided to use are:
* Jupyter notebook to conduct the training of the models.
* For the audio I decided to use pyaudio.
* For the NN will be the Tensorflow API.
* For the final aplication will be scripted in python.  
  
(These tecnologys are not finals and may change in the future)

I divided the project in 4 parts:
1. Create n number of samples to train the NN for recognicing the key-word. The samples are divided in "negatives" and "positives", at the moment im not quite sure how many of each I will need.
2. Experiment with different type of recursive NN structures to be able to predict when the computer recieves the activation word.
3. Ones the previous step is done, its time to create a data-set of words.
4. Here is either two options:
   1. Change the last layer of the previous NN to predict letters and form words.
   2. Use a whole new NN.
I will try to keep every thing explained in these README and in each notebook.

As for now the project its in the second part.
