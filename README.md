# DeepCaptchaSolver
DeepCaptchaSolver is a deep learning–based CAPTCHA decoding solution that leverages a custom Convolutional Neural Network (CNN) to efficiently process grayscale CAPTCHA images (100x50 pixels). The model accurately recognizes alphanumeric characters (A-Z, a-z, 0-9) using one-hot encoding, enabling real-time predictions.

This project implements a CAPTCHA recognition system using a Convolutional Neural Network (CNN). The model is trained to recognize alphanumeric CAPTCHA images and predict the correct text.

## Features
- Supports alphanumeric CAPTCHA recognition (A-Z, a-z, 0-9)
- Uses CNN for accurate text recognition
- Implements real-time CAPTCHA prediction
- Trained using TensorFlow and Keras
- Supports grayscale image processing

## Dataset
The dataset consists of CAPTCHA images labeled with their corresponding text. Each image is resized to **100x50 pixels** and converted to grayscale before training.

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/captcha-recognition.git
   cd captcha-recognition
   ```
2. Install required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Set up your dataset:
   - Place CAPTCHA images inside a directory (e.g., `D:\Dataset\samples`)

## Usage
### Training the Model
Run the following command to train the model:
```sh
python train.py
```

### Predict CAPTCHA
Use the trained model to predict a CAPTCHA:
```sh
python predict.py --image path/to/captcha.png
```

## Project Structure
```
├── captcha_recognition/
│   ├── train.py          # Training script
│   ├── predict.py        # Prediction script
│   ├── model/            # Saved model
│   ├── dataset/          # CAPTCHA images
│   ├── README.md         # Project description
│   ├── requirements.txt  # Dependencies
```

## Model Architecture
The model consists of:
- Convolutional layers for feature extraction
- MaxPooling layers for dimensionality reduction
- Dense layers for character classification
- Softmax activation for multi-character output

## Example Prediction
Example output from the model:
```sh
Predicted CAPTCHA: 2b827
```

## License
This project is open-source under the [MIT License](LICENSE).


