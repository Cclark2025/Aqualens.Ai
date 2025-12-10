📘 Project Overview

AquaLens AI is a computer vision project designed to improve water pollution monitoring through automated image classification. Using deep learning, the system idedntifies whether a water sample appears clean or polluted, offering a faster and more scalable alternative to traditional laboratory-based testing. The project aims to support environmental researchers, local governments, and communities by providing real-time, accessible water quality assessments.

🌍 Problem & Motivation

Water pollution is often difficult to detect without specialized laboratory testing, which leads to delays in identifying harmful contaminants. Traditional monitoring methods are:

Slow — results may take days or weeks

Expensive — requiring specialized equipment and trained personnel

Inaccessible — many rural or low-resource communities lack testing infrastructure

AquaLens AI provides a solution by applying deep learning to analyze water images directly. By classifying images as clean or polluted, it offers a faster, automated, and highly scalable approach to water quality assessment.

🧠 AlexNet Technical Approach

AquaLens AI uses a deep learning workflow centered around AlexNet, a convolutional neural network originally designed for large-scale image recognition. The project adapts AlexNet to classify water samples through:

Model Workflow

Dataset Structure:
433 total images, split into training and testing sets with two labels — clean and polluted.

Preprocessing:
Images are resized, normalized, and organized into labeled folders.

Training Pipeline:
AlexNet is trained for multiple epochs using cross-entropy loss and standard optimization techniques.

Augmentation Tests:
Experiments included testing AlexNet with and without data augmentation to compare generalization.

Vision

AquaLens AI ultimately aims to provide real-time, actionable environmental insights using scalable AI and computer vision.

📊 Results
Model Performance Overview

Three convolutional neural network architectures were evaluated:

AlexNet

VGG16

ResNet18

All models were trained for 5 epochs using identical training and validation splits. Validation accuracy served as the primary performance metric.

Data Augmentation Impact (AlexNet)

Without augmentation: ~89.6% accuracy

With augmentation: ~72.9% accuracy
➡️ Conclusion: AlexNet struggles when images are distorted, indicating limited generalization ability.

Best Architecture: ResNet18

Achieved ~89.6% accuracy consistently across epochs

Outperformed augmented AlexNet

Matched or exceeded AlexNet’s baseline performance

Overall Findings

ResNet18 is the strongest model, offering the best balance of accuracy and robustness.

AlexNet is sensitive to augmentation, suggesting it relies heavily on specific visual cues.

Model accuracy plateaued around 90%, which is strong given the small dataset size.

🚀 Takeaways & Future Work

Across all experiments, ResNet18 consistently delivered the highest accuracy and strongest generalization. Its residual learning framework enables the extraction of more stable visual features—such as turbidity, color shifts, and particulate patterns—making it more resilient to noise and variation in water imagery.

Key takeaways:

AlexNet performs well on raw images but loses accuracy when augmented, revealing limited robustness.

ResNet18 generalizes significantly better, making it the preferred architecture for future development.

Dataset size is a limiting factor; expanding it will likely push accuracy beyond 90%.

Future Improvements

Expand the dataset across seasons, lighting conditions, and geographic regions

Integrate advanced architectures like EfficientNet or Vision Transformers

Develop a user-facing web dashboard for real-time predictions

Implement multi-class classification (e.g., plastics, algae blooms, chemical discoloration)
