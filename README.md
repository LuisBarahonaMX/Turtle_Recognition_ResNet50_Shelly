# Turtle Recognition with ResNet50 and Shelly

![Project Cover](https://lh3.googleusercontent.com/BtTiv77ZlOgPbwcl_qQmqPp-CGyr3mSriE3WrXshQ-H69AKFd1Y_tKKhvUPLNbHLvytYmI5oT3-ZbTKvV5CrnEGcYgki5K2wREUIpQ4d9J0R-Chk=w1024-h576-n-nu-rw-lo)

### Transfer Learning, Computer Vision, and Experimental Wildlife Image Recognition

**Project Type:** Experimental AI / Computer Vision Notebook  
**Field:** Artificial Intelligence | Deep Learning | Computer Vision | Wildlife Recognition  
**Author:** Data Engineer Luis Barahona  
**Environment:** Google Colab | Jupyter Notebook

---

## 1. Project Overview

This project explores an experimental computer vision workflow for turtle image recognition using deep learning techniques.

The notebook focuses on image classification with **ResNet50** through transfer learning, while also exploring complementary tools from **Hugging Face**, including **Shelly** and **DETR**, to study additional possibilities for object understanding and image-based analysis.

The main purpose of the project is to investigate how pretrained deep learning models can be adapted for marine wildlife recognition tasks, especially in scenarios involving turtle photographs.

---

## 2. Project Objectives

- Build an experimental image classification pipeline for turtle recognition.
- Use **ResNet50** as a pretrained convolutional neural network backbone.
- Apply **transfer learning** to adapt the model to a custom turtle dataset.
- Prepare image data for training and validation.
- Evaluate model behavior using training and validation metrics.
- Test prediction workflows on sample images.
- Explore additional Hugging Face tools such as **Shelly** and **DETR**.
- Save trained model weights for future experimentation.

---

## 3. Notebook Scope

The notebook combines multiple exploratory tasks related to image recognition:

- Dataset loading from Google Drive or ZIP files.
- Image preprocessing and normalization.
- Data splitting into training and validation sets.
- Transfer learning with ResNet50.
- Experimental prediction on turtle images.
- Additional experiments with Hugging Face-based models.
- Preliminary object detection exploration using DETR.

This repository represents an **experimental phase** rather than a fully validated production system.

---

## 4. Methodology

### 4.1 Data Preparation

The workflow begins by loading turtle images stored in folders organized by class or identity.

Images are resized and transformed into tensors suitable for deep learning models.

### 4.2 Preprocessing

The notebook applies standard image preprocessing steps, including:

- Image resizing to 224 × 224 pixels
- Tensor conversion
- Normalization using ImageNet-style statistics

These transformations ensure compatibility with pretrained ResNet50.

### 4.3 Train / Validation Split

The dataset is divided into:

- **85% training**
- **15% validation**

This allows monitoring of training performance and basic generalization behavior.

### 4.4 Transfer Learning with ResNet50

A pretrained **ResNet50** model is used as the main classification backbone.

The final classification layer is adapted to match the number of target classes in the turtle dataset.

Training is performed using a modern optimizer such as **AdamW**, allowing the network to learn task-specific patterns from turtle images.

### 4.5 Model Evaluation

During training, the notebook monitors:

- Training loss
- Validation loss
- Accuracy

These metrics help assess the learning behavior of the model during experimentation.

### 4.6 Prediction Workflow

The notebook includes experimental prediction steps to test the trained model on selected images.

This stage helps verify whether the model can assign labels to unseen turtle images.

### 4.7 Additional Exploration with Hugging Face

The project also explores other tools and models:

- **Shelly** for additional model experimentation
- **DETR** for object detection exploration

These components are exploratory and should be interpreted separately from the ResNet50 classification workflow.

---

## 5. Technologies Used

| Technology | Purpose |
|:---|:---|
| Python | Programming language |
| PyTorch | Deep learning framework |
| Torchvision | Pretrained vision models and transforms |
| ResNet50 | Transfer learning backbone |
| Hugging Face Transformers | Additional experimental model integration |
| DETR | Object detection exploration |
| Pillow | Image processing |
| Matplotlib | Visualization |
| Google Colab | Cloud notebook environment |
| CUDA / GPU | Accelerated training |

---

## 6. Key Features

- Experimental image classification workflow
- Transfer learning with a pretrained ResNet50 model
- Image preprocessing pipeline
- Validation-based training monitoring
- Sample image prediction testing
- Exploratory integration of Hugging Face tools
- Preliminary wildlife computer vision experimentation

---

## 7. Google Colab

[Open the notebook in Google Colab](https://colab.research.google.com/drive/1777h88oXWt7AW6BgXA9mtuhk5YgGTh87)

---

## 8. Project Limitations

This project should be interpreted as an **experimental notebook**, not a finalized wildlife recognition system.

Important limitations include:

- The dataset size and structure may limit generalization.
- Validation is performed within the same broader dataset workflow.
- DETR-based exploration does not imply specialized turtle detection performance.
- Shelly-related experimentation is exploratory and separate from the core classifier.
- Real-world wildlife identification requires broader evaluation, stronger benchmarking, and domain-specific validation.

---

## 9. Potential Applications

This project can serve as a foundation for:

- Wildlife image classification
- Marine species monitoring
- Biodiversity research support
- Conservation technology experiments
- Transfer learning education in computer vision
- AI-assisted ecological analysis

---

## 10. Future Improvements

Possible next steps for this project include:

- Expanding the dataset with more turtle images
- Improving class balance
- Creating a stronger testing protocol with truly unseen images
- Comparing ResNet50 with other architectures
- Training a specialized object detector for turtles
- Integrating embeddings for individual turtle re-identification
- Building a cleaner inference pipeline for deployment

---

## 11. Conclusion

This notebook demonstrates an experimental deep learning approach for turtle image recognition using **ResNet50** and transfer learning.

It also broadens the exploration by testing additional Hugging Face-based tools such as **Shelly** and **DETR**.

Although the notebook is not yet a production-ready recognition system, it provides a meaningful foundation for future work in **wildlife computer vision**, **marine conservation technology**, and **AI-assisted ecological research**.

---

## Author

**Data Engineer Luis Barahona**

Mexican Data Engineer and 2026 graduate of Universidad del Caribe, interested in Artificial Intelligence, Data Science, Computer Vision, and technology-driven solutions for real-world problems.

---

## Contact

| Platform | Contact |
|:---|:---|
| Email | [190300395@ucaribe.edu.mx](mailto:190300395@ucaribe.edu.mx) |
| GitHub | [github.com/LuisBarahonaMX](https://github.com/LuisBarahonaMX) |
| LinkedIn | [linkedin.com/in/luis-barahona-mx](https://www.linkedin.com/in/luis-barahona-mx/) |
| Instagram | [@luisbarahonamx](https://www.instagram.com/luisbarahonamx/) |
| X | [@luisbarahonaMX](https://x.com/luisbarahonaMX) |
| Website | [SIKO AI Platform](https://sikoai.web.app/) |
