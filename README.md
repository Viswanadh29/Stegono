# Image-Based Steganography with OpenCV

## Overview
This project implements a simple image-based steganography technique using OpenCV in Python. It allows users to hide a secret message inside an image and retrieve it later using a passcode for decryption.

## Requirements
- Python 3.x
- OpenCV (`cv2`)
- OS module (`os`)

## Installation
Ensure you have Python installed on your system. Then, install OpenCV if it is not already installed:
```bash
pip install opencv-python
```

## Usage
### Encryption
1. Place the image file (`myimg.jpg`) in the same directory as the script.
2. Run the script and enter the secret message when prompted.
3. Provide a passcode for encryption.
4. The message will be encoded into the image.
5. The modified image (`encryptedImage.jpg`) will be saved and opened automatically.

### Decryption
1. Run the script again.
2. Enter the same passcode used during encryption.
3. If the passcode is correct, the hidden message will be revealed.
4. If the passcode is incorrect, access will be denied.

## Code Explanation
- The script reads an image using OpenCV.
- It maps ASCII characters to their corresponding integer values for encoding.
- The secret message is embedded into the image's pixel values.
- The same approach is used to extract the message when provided with the correct passcode.

## Limitations
- The message length is limited by the number of pixels available in the image.
- The encoding method is simplistic and not secure against advanced steganalysis techniques.
- Only basic ASCII characters are supported.

## Disclaimer
This project is for educational purposes only. It is not a secure encryption method and should not be used for sensitive data.
