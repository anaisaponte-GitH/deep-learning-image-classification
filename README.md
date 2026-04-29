# 🧠 Image Classification with CNN (Cats vs Dogs)

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify images of cats and dogs.

It is designed as a **portfolio project**, showcasing a complete deep learning workflow from data preparation to model evaluation.

---

## 🎯 Objective

The goal of this project is to build a deep learning model capable of learning visual patterns from images and generalizing to unseen data.

---

## 🛠️ Technologies

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## ⚙️ Approach

The project follows these main steps:

- Data preparation and validation
- Image preprocessing with `ImageDataGenerator`
- Lightweight CNN architecture design
- Training optimization with:
  - EarlyStopping
  - ModelCheckpoint
- Evaluation on validation data
- Qualitative analysis of predictions

---

## 📊 Results

- **Validation accuracy:** ~69%
- **Validation loss:** ~0.57

The model shows a clear improvement over the initial baseline and achieves a reasonable balance between simplicity and learning capacity.

---

## 📁 Repository Structure

```text
.
├── cnn_image_classification.ipynb
├── data/
│   └── raw/
│       └── dogs-vs-cats/
│           └── train/
├── README.md
├── LICENSE
└── .gitignore
```

---

## 📦 Dataset

The dataset is not included in this repository due to size limitations.

This project uses the public **Dogs vs. Cats** image classification dataset originally released through Kaggle/Microsoft.

You can download it from Kaggle:  [Dogs vs. Cats competition dataset](https://www.kaggle.com/c/dogs-vs-cats/data)

After downloading, place the images in the following directory:

data/raw/dogs-vs-cats/train

The images should be organized in two folders:

data/raw/dogs-vs-cats/train/cat/  
data/raw/dogs-vs-cats/train/dog/

The notebook expects images to be already organized in these folders.

If the folders are empty, the notebook will run but data loading cells will fail because no images are available.


---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/anaisaponte-GitH/deep-learning-image-classification.git
cd deep-learning-image-classification
```

### 2. Create virtual environment

```bash
python -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```
Dependencies are listed in `requirements.txt`.

### 4. Add dataset

For dataset details, see the Dataset section above.

Download the Cats vs Dogs dataset from Kaggle and place the images using the following structure:

```text
data/
└── raw/
    └── dogs-vs-cats/
        └── train/
            ├── cat/
            │   ├── cat.0.jpg
            │   ├── cat.1.jpg
            │   └── ...
            └── dog/
                ├── dog.0.jpg
                ├── dog.1.jpg
                └── ...
````

The notebook expects the images to be available at:
```text
data/raw/dogs-vs-cats/train/
```

with two subfolders: cat/ and dog/.

### 5. Run notebook

```bash
jupyter notebook cnn_image_classification.ipynb
```
Then open the notebook and click **"Run All"** to execute the full pipeline.

---

## 📈 Possible Improvements

- Data augmentation to improve generalization
- Hyperparameter tuning
- Transfer learning (e.g., MobileNet, VGG16)
- Larger dataset
- Better regularization techniques

---

## 💼 Notes for Recruiters

This project demonstrates:

- End-to-end deep learning workflow
- Practical use of TensorFlow/Keras
- Ability to structure a clean and reproducible project
- Understanding of CNN fundamentals
- Clear documentation and communication of results

---

## 👩‍💻 Author

Ing. Anais Aponte