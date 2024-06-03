# Handwriting Recognition using ML

This project involves building a handwriting recognition system using machine learning. The model is trained on the MNIST dataset, which consists of 60,000 training images and 10,000 testing images of handwritten digits.

## Features

- Train a machine learning model to recognize handwritten digits
- Use the MNIST dataset for training and testing
- Evaluate the performance of the model

## Model Architecture

The model is a Convolutional Neural Network (CNN) with the following architecture:

```
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 conv2d (Conv2D)             (None, 26, 26, 32)        320       
                                                                 
 max_pooling2d (MaxPooling2D  (None, 13, 13, 32)       0         
 )                                                               
                                                                 
 conv2d_1 (Conv2D)           (None, 11, 11, 32)        9248      
                                                                 
 max_pooling2d_1 (MaxPooling  (None, 5, 5, 32)         0         
 2D)                                                             
                                                                 
 flatten (Flatten)           (None, 800)               0         
                                                                 
 dense (Dense)               (None, 512)               410112    
                                                                 
 dense_1 (Dense)             (None, 26)                13338     
                                                                 
=================================================================
Total params: 433,018
Trainable params: 433,018
Non-trainable params: 0
_________________________________________________________________
```

## Requirements

To run this project, you will need the following packages:

- numpy
- pandas
- matplotlib
- scikit-learn
- tensorflow or keras

You can install the required packages using the following command:

```bash
pip install -r requirements.txt
```
## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
