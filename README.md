# Food-Image-Classification
Image classification is an active area of research and development in deep learning where many milestones are continuously being attained. Applications of such technology varies from areas of defense and security to facial recognition to labeling items in e-commerce etc. 

In this study we are presented with tensor flow dataset named food101, containing 750 images of food data for 101 classes of food each,  to come up with a deep learning model/algorithm to correctly classify the food from the image. This is useful to determine the intake of food to evaluate the effectiveness of any dietary interventions. This dataset and previous research for image classification approaches is specifically targeted towards determining the effective of nutritional and dietary interventions of obese individuals whose diet has to be monitored closely. 

Our proposed models are based on Convolutional Neural Network (CNN). We built the model using transfer learning with EfficientNetB0 as the base model. We further fine-tuned the model based on the images in our food-101 dataset. The fine-tuned model has been able to predict the image classes with ~80% accuracy and has been able to utilize mixed-precision training (MPT) available in transfer flow. This boosted the model’s computational performance by 3X with GPU amounting to about 300 secs per epoch with Tesla T4 GPU. Learning rate of 1e-4 was optimal during fine-tuning with all layers unfrozen of the EfficientNetB0 model with higher/default learning rates leading to vanishing/gradient blowout issues.
 
The accuracy of the model could be improved by other fine-tuning option like unfreezing few layers at a time, using transfer learning with more advanced EfficientNet models like EfficientNetB4 and tuning the learning rates.

Keywords: Food image classification, deep learning, Convolutional Neural Network, dietary assessment

Link to Notebook: https://github.com/R-Madhuram/Food-Image-Classification/blob/main/Food_Vision_101.ipynb
