# Hair-Texture-Identifier
![Logo](curly_hair.png)

Harness the latest advancements in artificial intelligence to precisely distinguish between curly and straight hair, revolutionizing the way you discover hair care products tailored to your unique hair texture.

## Problem
Data Bias: AI systems, including those used in e-commerce and search engines, heavily rely on vast datasets to make decisions. If these datasets are biased towards straight hair or lack diverse representations of different hair types, the AI may struggle to understand and cater to the unique needs of those with curly hair. The bias in training data can result in inaccurate recommendations.

Complexity of Hair Textures: Curly and straight hair types exhibit a wide range of textures, patterns, and variations. The subtle differences between these types can be challenging for AI algorithms to discern, especially if the training data does not cover the full spectrum of these variations. Curly hair can have different curl patterns (from loose to tight curls), while straight hair can also vary in thickness and texture.

Lack of Contextual Understanding: AI systems often lack the ability to understand the context of a user's query or the specific needs of individuals with curly hair. Recommendations may be based solely on keyword matching, disregarding the nuances of the user's requirements.

Limited User Feedback: Machine learning models continuously improve by learning from user feedback. If users with curly hair consistently receive straight hair product recommendations and do not provide corrective feedback, the AI system may never learn to differentiate between the two effectively.

Inadequate Image Recognition: In cases where users search for hair products using images (e.g., a picture of their own hair), AI image recognition may not accurately classify the hair type. This can result in mismatched recommendations.

Addressing this problem requires improvements in AI training data, more inclusive datasets, and enhanced machine learning algorithms that can better distinguish between different hair types. Additionally, refining contextual understanding and user feedback mechanisms can help AI systems provide more accurate and personalized recommendations for individuals with curly hair. As AI technology continues to evolve, efforts to reduce bias and improve the recognition of diverse hair types will be essential to ensure fair and effective user experiences in the realm of beauty and personal care products.

## Solution
Using google colab I implemented these types of code: 
Loading Labels and Pre-trained Model: It loads labels for the model's classes and initializes a pre-trained AlexNet model.

Downloading Google Slides Images: It fetches images from a Google Slides presentation by first downloading the presentation as a PDF and then converting PDF pages to images.

Data Preprocessing: The images are preprocessed, resized, and normalized to prepare them for input to the model.

Model Inference: It uses the pre-trained AlexNet model to make predictions on the processed images.

Classification Results: The code determines the model's predictions and prints the corresponding labels for each image. It also appears to be setting up some binary classification data, but it's unclear how it's being used in the context of the code.

Data Conversion and Preparation: The code sets up some data arrays and reshapes them for further processing.

Defining Loss Functions: The code defines a softmax function and a cross-entropy loss function.

Random Number Generation: It defines functions for generating random numbers and truncated normal random numbers.

Training Loop: A training loop is initiated with a set number of epochs. Within each epoch, a batch of training data is fetched. The cross-entropy loss is computed and backpropagation is performed to update the model's weights. The loss and other metrics are logged using Weights and Biases (wandb).

Initialization and Configuration: It initializes the Weights and Biases project and sets various configuration parameters such as learning rate, batch size, and the number of training epochs.

Optimization and Logging: The code enters the training loop, where the model is updated using the Adam optimizer, and loss and accuracy metrics are logged.

## Data Deck
[Data_Deck](https://docs.google.com/presentation/d/1mATs77DNphkXvP1BRh-J_wFg3ptQ-K5wyM0xJHjR4pk/edit?usp=sharing)

## Alexnet Filters
[Alexnet Filters](https://colab.research.google.com/drive/1h5G64TCkruibmEOqh0kwUp_-pb3AKZp4?usp=sharing)
