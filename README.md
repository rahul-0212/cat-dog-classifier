🐱🐶 Cat vs Dog Image Classifier

A simple web application built using Flask and a pre-trained TensorFlow/Keras model to classify uploaded images as either a cat or a dog.

🚀 Features

Upload an image through a web interface

Deep learning model classifies the image

Outputs prediction: Cat 🐱 or Dog 🐶

Includes routes: Home, About, Contact, and Project (upload page)

📁 Project Structure
├── static/Data/images/       # Sample images (optional)
├── templates/                # HTML files: index.html, about.html, contact.html, project.html
├── app.py                    # Flask web server
├── model.h5                  # Pre-trained Keras model
├── cat_dog.ipynb             # Notebook used for training the model
├── README.md                 # Project documentation
├── LICENSE

⚙️ Setup Instructions

Clone the repo:

git clone https://github.com/rahul-0212/cat-dog-classifier.git
cd cat-dog-classifier


Install dependencies:

pip install -r requirements.txt


(Make sure to include a requirements.txt file with packages like Flask, TensorFlow, Pillow, etc.)

Run the app:

python app.py


Open in browser:
Visit http://127.0.0.1:5000/

🧠 Model Details

The model expects input images resized to 224x224 pixels.

It outputs a single sigmoid value:

0.5 = Dog

≤ 0.5 = Cat

📷 How It Works

Upload an image via the /project route.

Image is preprocessed (resized and normalized).

Model predicts the class.

Prediction is displayed on the webpage.

Uploaded image is deleted after classification.

📄 License

This project is licensed under the MIT License.
