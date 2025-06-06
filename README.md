# Problem - Image classification with Deep neural network

Solution :-

  > Network/Layer - DenseNet121

  > Framework - Caffe

  > Dataset (while training the network) - ILSVRC2012

  > Library - cv2, numpy, matplotlib.pyplot 

  > Pipeline (Inderfence/testing) :-

      : Read the image.

      : Extract the class names from the class file- ILSVRC2012 dataset.

      : Load the network's model file (stored trained weights). 
      
      : Load the network's config file (stored network's configuration / architexture detail).

      : Read the network's files using Caffe framework.

      : Convert the image into blob format- helps the network to understand the image through blob format. 
        Note- the parameters of blob function to convert image into blob is as per the newtwork's configuration text file.
      
      : Set the blob image ready and pass the blob forward to the to the loaded model.

      : Receive the first layer from the output layers and flatten the layer wrt number of classes (1000)- this layer consists of the classification scores of all classes wrt to an input image

      : From the flatten layer, search for the class's index and the score who has maximum classification score.

      : Display the maximum score and the class name (help of class's index)- as these are the accuracy values of claasifying the input image into its respective classes.
