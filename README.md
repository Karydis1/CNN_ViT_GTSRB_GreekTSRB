# Traffic Sign Classification using CNN & Vision Transformers (GTSRB & GreekTSRB)

##  Overview
This project focuses on traffic sign classification using deep learning techniques, including Convolutional Neural Networks (CNNs) and Vision Transformers (ViTs).

The main objective is to evaluate model performance across different datasets and study generalization from German traffic signs (GTSRB) to Greek traffic signs (GreekTSRB).

##  Objectives
- Train deep learning models for traffic sign classification
- Evaluate cross-dataset generalization (German → Greek signs)
- Improve performance using dataset augmentation and mixing
- Compare different model architectures (CNN vs ViT)

##  Datasets
- **GTSRB** (German Traffic Sign Recognition Benchmark)
- **Greek Traffic Sign Dataset (GreekTSRB)**

Each dataset contains labeled traffic sign images with multiple classes.

##  Methodology

###  Data Preprocessing
- Data shuffling
- Grayscale conversion
- Local histogram equalization
- Normalization
- Dataset splitting (train / validation / test)

###  Models
- Convolutional Neural Networks (CNNs)
- Vision Transformer (ViT) architectures

###  Experiments
1. Train on German dataset → Test on Greek dataset  
2. Train on mixed dataset (German + Greek) → Test on Greek dataset  
3. Train only on Greek dataset  
4. Model simplification and optimization for better performance  

##  Results

- Training on **German dataset only** → Test on Greek signs:  
   Accuracy: **~67–73%**  
  → Poor generalization to Greek road conditions  

- Training on **mixed dataset (German + Greek)** → Test on Greek signs:  
   Accuracy: **~96%**  
  → Significant improvement due to dataset adaptation  

- Training on **Greek dataset only**:
  → Further improvements with optimized architecture  

##  Key Insights
- Models trained on one domain do not generalize well to another without adaptation
- Dataset diversity is critical for real-world performance
- Combining datasets significantly improves accuracy
- Simpler architectures can outperform complex ones when properly tuned

##  Technologies Used
- Python
- TensorFlow / Keras (or PyTorch if applicable)
- NumPy / Pandas
- OpenCV
- Matplotlib
- Jupyter Notebook

##  Visualization
- Training / validation accuracy plots
- Sample predictions
- Dataset exploration

##  Future Improvements
- Use of data augmentation techniques
- Transfer learning with pretrained models
- Real-time traffic sign detection (video input)
- Deployment in embedded or autonomous driving systems

## 📌 Notes
This project highlights the importance of domain adaptation in computer vision applications, especially in real-world environments like autonomous driving.
