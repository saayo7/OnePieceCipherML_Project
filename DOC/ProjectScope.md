# One Piece Project

## Data

Go to the directory called DATA

## Websites to read

### Context & Info

[Site1:](https://cipherfoundation.org/older-ciphers/la-buse-cryptogram/)
[Site2:](https://sites.google.com/view/labuse)

## Project Scope

This project aims to develop a machine learning pipeline that can automatically translate and decrypt images of ciphers, specifically inspired by the historical cipher of Olivier Levasseur. The project will leverage a Convolutional Neural Network (CNN) to recognize and classify symbols from the cipher. Additionally, a secondary machine learning model (e.g., a Recurrent Neural Network or Transformer) will be employed to directly decrypt the sequence of recognized symbols into plaintext, or the CNN will be extended to include a decryption layer that interprets the symbols in context.

## Objectives

1. **Data Preprocessing**

    - Segment the provided cipher image into individual symbols.
    - Preprocess the symbols (e.g., binarization, resizing) to prepare them for input into the CNN.
2. **CNN Model Development**

    - Design and implement a CNN architecture capable of recognizing and classifying the segmented symbols.
    - Train the CNN on a labeled dataset of cipher symbols to predict corresponding plaintext characters or intermediary cipher text.
3. **Decryption via ML**

    - **Option 1: Integrated CNN Decryption**
        - Extend the CNN model to include additional layers that handle the decryption of the sequence of symbols, effectively combining recognition and decryption in one model.
    - **Option 2: Secondary Decryption Model**
        - Develop a separate machine learning model (such as an RNN or Transformer) that takes the sequence of recognized symbols as input and outputs the decrypted text.
        - Train this model using sequences of ciphered symbols paired with their corresponding plaintext translations.
4. **Testing and Evaluation**

    - Test the combined model or the sequential model pipeline on unseen cipher images to evaluate its accuracy in both symbol recognition and decryption.
    - Fine-tune the models based on test results, ensuring the decryption process is both accurate and efficient.
5. **Deployment**

    - Package the end-to-end decryption pipeline for deployment as a standalone application or web service.
    - Develop a user interface to allow users to upload cipher images and receive decrypted text directly.

## Final Thoughts

Inspired by Olivier Levasseur's cryptogram and "One Piece," this project integrates decryption into a CNN or secondary model, creating a tool that recognizes and deciphers complex ciphers. It merges ancient mysteries with modern ML, unlocking new possibilities.

## Future Work

For future work, I would like to extend the model to take plaintext input and generate an image resembling the original cipher, effectively reversing the decryption process and creating a complete cycle of translation and generation.
