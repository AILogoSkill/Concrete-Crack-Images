# Concrete-Crack-Images
![image](https://github.com/AILogoSkill/Concrete-Crack-Images/assets/144710374/60ca3747-2e61-44fb-8c42-a087ea9f7c61)


Concrete is perhaps the most widely used building material globally and is one of the most important materials in civil construction, including its use in road construction. Strength is one of the main reasons concrete has been used in construction for many decades. It can easily handle loads associated with tension and compression without succumbing to their effects. Concrete is exceptionally robust and can last for many years, enduring harsh weather conditions and natural disasters, as it is rigid and resistant to deformation. However, these characteristics also mean that concrete structures lack flexibility and are unable to withstand environmental changes. The appearance of cracks is usually the first sign of concrete damage, and deterioration may occur before more significant defects become apparent.

# Problem Statement

Cracks on the surface of concrete are a serious defect for any civil structures (not just roads, but also buildings, bridges, etc.). If not addressed in a timely manner, these defects can not only have a detrimental impact on the structural condition and durability but can also lead to large-scale disasters, including fatal accidents. To prevent accidents, regular inspections of various concrete structures are necessary. Structural inspections are conducted to assess the stiffness and strength of the structure under stress. This is usually done by checking the concrete for cracks. Depending on the condition of the surface, a decision is made to replace the damaged area with new material. To detect cracks, potholes, damage to joints, and other defects that compromise the integrity and strength of the road surface, an automated system needs to be developed that can effectively recognize the presence of defects.

# Project Objective

The goal is to create a deep learning model using a Convolutional Neural Network (CNN) algorithm that alerts about defects in concrete. A Convolutional Neural Network is a class of deep neural networks most commonly applied to the analysis of visual imagery. In this project, Keras is used, an open-source software library that provides a Python interface for artificial neural networks, particularly convolutional networks.

# Methodology

The task is to solve an image classification problem, which involves providing an image as input to a model built using a specific algorithm, which outputs the class label or probability of the class to which the image belongs. This process falls under supervised learning. The Convolutional Neural Network algorithm is primarily used for visual imagery. The CNN model consists of two main parts. The first part consists of convolutional layers and pooling layers, where the main process of feature extraction takes place. In the second part, fully connected layers perform several non-linear transformations of the extracted features and act as part of the classifier.

# Dataset

To address the given problem, the dataset from Mendeley is proposed, consisting of images, half of which contain cracks in concrete. The dataset was published on June 23, 2019, and the data was collected in various buildings on the Middle East Technical University campuses. The original collected images with cracks in the concrete in the specified dataset total 2000, but to obtain a model with good performance, generalization to previously unseen instances of data, and high accuracy, such a quantity of data is insufficient. Additionally, the resolution of the original images is 1024 × 1024 pixels, which would result in too much memory overhead when using instances of the dataset as input data for the model. For this reason, all images from the input dataset were compressed to a size of 227 × 227 pixels, and the dataset was artificially increased to 40,000 instances. The dataset is divided into two parts: "negative" (without defects) and "positive" (with defects) concrete images, with 20,000 color (RGB) images for each class. Thus, for defect recognition, a binary classification task needs to be solved.

