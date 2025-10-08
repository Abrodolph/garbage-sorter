## ♻️ AI-Powered Garbage Sorter

A web application that uses a deep learning model to classify garbage into different categories. This tool helps users correctly sort their waste by simply uploading an image.

## ✨ Key Features

Image-Based Classification: Upload an image of any waste item to get an instant classification.

Multiple Categories: The model is trained to recognize a wide range of garbage types, including glass, paper, cardboard, plastic, metal, and more.

Simple Web Interface: A clean and intuitive user interface built with Flask makes it easy for anyone to use.

Deep Learning Model: Powered by a robust Convolutional Neural Network (CNN) built with TensorFlow and Keras.

## ⚙️ How It Works
The application workflow is straightforward:

Image Upload: The user selects an image of a garbage item and uploads it through the web interface.

Image Preprocessing: The backend receives the image and preprocesses it to match the input requirements of the machine learning model (e.g., resizing to the correct dimensions).

Model Prediction: The preprocessed image is passed to the pre-trained Keras model (final_model.h5). The model analyzes the image and predicts the probability for each garbage category.

Display Results: The category with the highest probability is identified, and the result is sent back to the user and displayed on the prediction page.

## 🛠️ Tech Stack

Backend: Python, Flask

Machine Learning: TensorFlow, Keras, Pillow

Frontend: HTML, CSS (from templates/ and static/ directories)

## 🗂️ Dataset

The model was trained on the "Garbage Classification" dataset, which contains images sorted into the following categories:

Battery

Biological

Brown Glass

Cardboard

Clothes

Green Glass

Metal

Paper

Plastic

Shoes

Trash

White Glass

The dataset is located in the garbage_classification/ directory of this repository.

## 🔧 Setup and Local Installation
To run this project on your local machine, follow these steps:

1. **Clone the repository:**

    ```sh
    git clone https://github.com/Abrodolph/garbage-sorter.git
    cd garbage-sorter
    ```

2. **Create and activate a virtual environment:**

```sh
python -m venv venv
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate
  ```
  
3. **Install the required dependencies:**

  ```sh
pip install -r requirements.txt
  ```
  
4. **Run the application:**

  ```sh
python app.py
  ```
  
The application will be available at http://127.0.0.1:5000.

📄 License
This project is distributed under the MIT License. See LICENSE for more information.

