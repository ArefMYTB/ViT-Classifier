# Vision Transformer (ViT) from Scratch on CIFAR-10

This project implements a **Vision Transformer (ViT)** from scratch in PyTorch and trains it on the **CIFAR-10 dataset**.  

---

## Project Highlights
- Built **ViT architecture** completely from scratch (no HuggingFace or timm shortcuts).  
- Implemented **patch embedding**, **multi-head self-attention**, **MLP blocks**, and **positional embeddings**.  
- Trained on **CIFAR-10** (45k images for training, 5k images for validation and 10k for testing - 10 classes).  
- Achieved **67.41% test accuracy** after ~45 minutes.  
- Visualized:
  - Training loss & accuracy curves  
  - Predictions on sample images  
  - Learned positional embeddings  

---

## Results

### Training Loss
<img width="835" height="451" alt="image" src="https://github.com/user-attachments/assets/0b163243-56c3-475e-9e5a-9fcfa9d98622" />


### Accuracy (Train vs Validation)
<img width="835" height="451" alt="image" src="https://github.com/user-attachments/assets/3cbd0cc2-c66c-4b65-aad5-fb6d0567e66a" />

### Final Test Accuracy
The total test accuracy is: 67.41%


### Sample Predictions
<img width="1280" height="230" alt="image" src="https://github.com/user-attachments/assets/1bed6bb3-481c-4a9e-b84f-422a76619041" />

### Positional Embedding Visualization
<img width="489" height="490" alt="image" src="https://github.com/user-attachments/assets/d49d55c6-fb5b-4fb5-9b98-4c0f608552bc" />

---

## Training Setup
- **Environment**: Google Colab (Tesla T4 GPU)  
- **Training time**: ~45 minutes  
- **Epochs**: 30  
- **Batch size**: 128  
- **Optimizer**: Adam + CosineAnnealingLR  
- **Loss function**: CrossEntropyLoss  
