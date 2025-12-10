---
1. Project Overview

A brief introduction to the AquaLens AI project and what it aims to accomplish.

2. Problem & Motivation

Why water pollution detection matters and what inspired this project.
Water pollution is often difficult to detect without specialized laboratory testing, leading to delays in identifying harmful contaminants. Traditional monitoring methods are time-consuming, expensive, and inaccessible in many communities. Aqualens AI aims to solve this problem by using deep learning to classify clean versus polluted water from images, providing a faster, automated, and scalable approach to water quality assessment.


3. AlexNet Technical Approach

A clear summary of how AlexNet is used, including preprocessing and training steps.

AquaLens AI harnesses cutting-edge artificial intelligence and computer vision to revolutionize water pollution detection and monitoring. We provide real-time, actionable insights to protect our planet's most vital resource.

Aqualens AI uses a deep learning workflow to classify water images as clean or polluted. The primary model is AlexNet, a convolutional neural network trained on standardized water images that were resized and normalized for consistency. The dataset is structured into separate train and test folders, each containing labeled images of clean and polluted water. 
Data set 433 images split into 




5. Results
Model Performance Overview
Three convolutional neural network (CNN) architectures—AlexNet, VGG16, and ResNet18—were evaluated to classify water images into Clean and Dirty categories.
 Each model was trained for 5 epochs using identical training and validation splits, and evaluated using validation accuracy as the primary performance metric.
Effect of Data Augmentation (AlexNet)
Result: Validation Accuracy decreased from ~89.6% (no augmentation) to ~72.9% (with augmentation)
ResNet18 Architecture Performance (Best Model)
Result: ResNet18 achieved ~89.6% accuracy consistently across epochs, outperforming AlexNet with augmentation and matching the AlexNet baseline.
 Overall Findings
ResNet18 is the top-performing architecture, providing the best balance of accuracy and generalization.
AlexNet suffers under augmentation, indicating the visual patterns defining “clean” vs “dirty” water are easily disrupted
Model accuracy plateaued around 90%, which is strong performance given the small dataset size.




Model accuracy, evaluation metrics, and key findings from the experiments.

6. Takeaways & Future Work
cross all experimental conditions, ResNet18 consistently demonstrated the strongest performance in classifying clean versus contaminated water samples, achieving validation accuracies approaching 90%, outperforming both AlexNet and VGG16 under identical training settings. While AlexNet performed reasonably well without augmentation, its accuracy dropped sharply when exposed to data perturbations, indicating sensitivity to visual distortions and limited generalization capacity on small datasets. In contrast, ResNet18’s residual learning architecture enabled it to extract more stable and discriminative features—particularly those related to turbidity, color gradients, and particulate patterns—resulting in superior robustness and accuracy.

Final reflections on what you learned and the next steps for improving the model.
