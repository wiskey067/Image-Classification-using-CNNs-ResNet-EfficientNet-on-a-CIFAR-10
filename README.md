
📌 Project: Image Classification using CNN, ResNet-50, and EfficientNet-B0 on CIFAR-10

This project explores image classification on the CIFAR-10 dataset using three different deep learning architectures:
	•	Simple CNN (baseline)
	•	ResNet-50 (deep residual network with skip connections)
	•	EfficientNet-B0 (optimized scaling-based model)

🚀 Objective

To compare the performance of traditional CNNs with modern architectures (ResNet and EfficientNet) and analyze trade-offs in accuracy, complexity, and training time.

📂 Dataset
	•	CIFAR-10: 60,000 images (32×32 RGB) across 10 classes
	•	Training: 50,000 images | Test: 10,000 images

🛠️ Implementation
	•	Framework: TensorFlow/Keras
	•	Loss Function: Categorical Crossentropy
	•	Optimizer: Adam/SGD
	•	Batch Size: 1560 (custom setting)
	•	Epochs: CNN (25), ResNet-50 (20–25), EfficientNet-B0 (30–40)
	•	Used early stopping to prevent overfitting

📊 Results

Model	Test Accuracy
CNN	70.52%
ResNet-50	71.77%
EfficientNet-B0	72.57%

Observation:
	•	EfficientNet-B0 slightly outperformed ResNet-50 and CNN.
	•	Trend: CNN < ResNet-50 < EfficientNet-B0
	•	Results show the impact of architecture depth and scaling efficiency.

✅ Key Takeaways
	•	Even without pretrained weights, deep architectures achieve decent accuracy on CIFAR-10.
	•	EfficientNet converges faster with fewer parameters compared to ResNet-50.
	•	Simple CNN provides a quick baseline but struggles with complex features.

📌 Future Improvements
	•	Use data augmentation (random crop, flip, rotation, cutout).
	•	Experiment with pretrained weights (ImageNet) for transfer learning.
	•	Fine-tune with learning rate schedulers (cosine annealing, OneCycle).
	•	Try CIFAR-100 for more challenging classification.

