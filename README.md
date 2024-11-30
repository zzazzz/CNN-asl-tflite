
# ASL Classification Using CNN

This project uses a **Convolutional Neural Network (CNN)** to classify American Sign Language (ASL) gestures into 36 categories (A-Z, 0-9).

## Project Structure
```
model_tfjs/         # TensorFlow.js model files
    ├── model.json
    ├── group1-shard1of1.bin
saved_model/        # TensorFlow SavedModel format
    ├── saved_model.pb
    ├── variables
tflite/             # TensorFlow Lite files for mobile deployment
    ├── label.txt  
    ├── model.tflite 
notebook.ipynb      # Jupyter Notebook for training and evaluation
requirements.txt    # Python dependencies
```

## Model Architecture
- **Convolutional Layers**: Extract features from images.
- **Pooling Layers**: Reduce spatial dimensions.
- **Dense Layers**: Classify the gestures into categories.

## Training Configuration
- **Input Shape**: 64x64 RGB images
- **Optimizer**: Adam
- **Loss**: Categorical Crossentropy
- **Metrics**: Accuracy

## Deployment
The model is converted into **TFLite** and **TensorFlow.js** formats for compatibility with mobile and web applications.

## How to Use

1. Clone Repository
   ```bash
   git clone https://github.com/zzazzz/ASL-Classification.git
    cd ASL-Classification
   ```
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook to train or evaluate the model.
4. Use the `model.tflite` for deployment on mobile devices.

---

Feel free to contribute or suggest improvements! 🎉
