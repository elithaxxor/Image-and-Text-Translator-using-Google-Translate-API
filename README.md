Image and Text Translator using Google Translate API


This Python project is designed to extract text from images and translate it into multiple languages using the Google Translate API. It uses a combination of image processing libraries and text extraction techniques to handle image-to-text conversions and provides various translation options.
	•	The googletrans version is specified due to the working release 4.0.0-rc1 for proper translation functionality.
Features

	•	Image to Text Extraction: Extract text from images using pytesseract and easyocr.
	•	Text Translation: Translate the extracted or input text to multiple languages including English, Spanish, French, and Latin.
	•	TextBlob Integration: Detect and handle the language of the input text.
	•	Multiple Language Support: Supports translation to various languages using Google Translate and TextBlob.
	•	Interactive Interface: Provides a command-line interface for user input, allowing the user to enter text or image locations for translation.

How It Works

	1.	Image Input: The program takes an image file as input from the user.
	2.	Text Extraction: The text in the image is extracted using OCR libraries (pytesseract and easyocr).
	3.	Translation: The extracted text or user-provided text is then translated into different languages using the Google Translate API and TextBlob.
	4.	Result Display: The translated text is displayed back to the user in the chosen language.

Installation

Prerequisites

Ensure you have Python installed on your machine.

Step 1: Clone the Repository
``` git clone https://github.com/yourusername/img-text-translator.git```

Step 2: Change Directory

``` cd img-text-translator
```
Step 3: Install Dependencies
```pip install -r requirements.txt
```
Here is the content of the requirements.txt:
```
    opencv-python
    pytesseract
    googletrans==4.0.0-rc1
    textblob
    easyocr
    Pillow
```

Make sure you have Tesseract OCR installed on your machine. You can download it from here.

Step 3: Install Tesseract OCR

	1.	Download and install Tesseract OCR from its official website.
	2.	Ensure that pytesseract.pytesseract.tesseract_cmd points to the correct Tesseract executable location.

Usage

Running the Program

To run the program, execute the following command:
    
    ```python main.py```

Instructions

	1.	Text Translation:
	•	Input the text you want to translate when prompted.
	•	The program will detect the language and translate it to English (or other languages, depending on the function you call).
	2.	Image to Text Translation:
	•	When prompted, input the location and name of the image file.
	•	The program will extract the text from the image, detect its language, and provide the translated text.

Example:
```angular2html

[+] Input the text for translation
:Enter the text for translation:
Hola amigos!
Detected Language: Spanish
Translated Text: Hello friends!
```
Code Overview

Key Components:

	1.	Text Translation (TextTranslate Class):
	•	Detects the language of the input text and provides translation options for multiple languages.
	2.	Image Processing (ImageTranslate Class):
	•	Reads and processes the input image, extracts text using OCR, and translates the text.
	3.	Color Formatting (Colors Class):
	•	Adds color formatting to the command-line interface to improve readability.


Known Issues

	•	Google Translate API Limitations: The free Google Translate API used in this project may have usage limits. For extended usage, consider integrating a paid translation service.
	•	Tesseract Accuracy: The accuracy of text extraction may vary depending on the quality of the image. Preprocessing the image with blurring or resizing can improve OCR results.

	•	The googletrans version is specified due to the working release 4.0.0-rc1 for proper translation functionality.
License

This project is open-source and free to use. All rights reserved by the author.

This project offers a basic framework for extracting text from images and translating it using various libraries. It is intended to serve as a foundation for more advanced image-to-text translation projects or applications.