# Image Encryption and Decryption Tool

## Overview
This repository contains a simple Python tool for encrypting and decrypting image files using a basic XOR operation. The tool allows users to securely handle images by applying a key for both encryption and decryption processes.

## Files
- `sample.jpg`: A sample image used for testing encryption and decryption.
- `image_encrypt_decrypt.py`: The Python script that contains the encryption and decryption logic.

## Code Explanation

### Function: `endec(path, key)`
This function takes the path of the image file and a key as inputs. It performs the following steps:

1. Opens the specified image file in binary read mode.
2. Reads the image content as a stream of bytes.
3. Converts the byte stream into a mutable array.
4. Applies the XOR operation between each byte and the specified key.
5. Writes the modified byte array back to the image file in binary write mode.

### User Interaction
The script prompts the user to select an action:
- **1** for encryption
- **2** for decryption
- **3** to exit

Depending on the user’s choice, the script will ask for the image path and the encryption/decryption key. 

## Sample Usage
To use the tool, run the following command in your terminal:

```bash
python image_encrypt_decrypt.py
