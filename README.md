# *HOROVODE-Keras*

   # *Distributed Deep Learning with Horovod*
    training of deep learning CNN model on MNIST dataset using Horovod Technique enabling faster, easier distributed training in TensorFlow.
    it employs efficient inter-GPU communication via ring reduction  

# *Files*:

    Horovod.pdf: Research paper explaining Horovod technique
    
    distributed_deep_learning_with_horovod.py: code for integrating horovod with Tensorflow keras.
                 
                 load_dataset  : loading MNIST dataset and converting those into trainX , trainY , testX , testY
             
                 prep_pixel    : converting train , test into float32 and dividing those into 255
                 
                 define_model  : designing model
                               
                                 Conv2D(32, (3, 3), activation='relu', kernel_initializer='he_uniform', input_shape=(28, 28, 1)))
                                 
                                 MaxPooling2D((2, 2))
                                 
                                 Flatten()
                                 
                                 Dense(100, activation='relu', kernel_initializer='he_uniform')
                                 
                                 Dense(10, activation='softmax')
                                 

# *Libraries*:

    tensorflow == 2.4.1
    Numpy      == 1.19.5
    sklearn    == 1.0.2
    matplotlib == 3.1
    horovod    == 0.25.0
    
