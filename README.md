# KannadaTextRecognizer
A Python-based tool that enables searching handwritten Kannada text in scanned PDF documents. It utilizes OCR (Optical Character Recognition) with Tesseract, along with image preprocessing, to extract and highlight searched phrases in the document. The project is built using libraries like pdf2image, OpenCV, pytesseract, and others.



# Kannada Handwritten Text Search

This project is a Python-based tool for searching handwritten Kannada text in scanned PDF documents. Using Optical Character Recognition (OCR), the program extracts Kannada text from the images in the PDF and highlights the searched phrases in the document. 

## Features
- Upload Kannada handwritten documents in PDF format.
- Extract Kannada text from scanned document images.
- Search for phrases in the extracted text.
- Highlight the found phrases on the scanned document pages.
- Display the processed images with highlighted search results.

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/YourUsername/KannadaHandwrittenTextSearch.git
    cd KannadaHandwrittenTextSearch
    ```

2. Install the required dependencies:
    ```bash
    pip install pdf2image opencv-python-headless numpy scipy pytesseract
    apt-get install -y poppler-utils tesseract-ocr tesseract-ocr-kan
    ```

## Usage

### In Google Colab
1. Open [Google Colab](https://colab.research.google.com/).
2. Upload this code in Colab or copy-paste the code directly.
3. Install the required libraries in Colab:
    ```python
    !pip install pdf2image opencv-python-headless numpy scipy pytesseract
    !apt-get install -y poppler-utils tesseract-ocr tesseract-ocr-kan
    ```
4. Run the notebook to:
   - Upload a PDF with Kannada handwritten text.
   - Index the document by extracting text from each page.
   - Search for specific phrases in the document and highlight them on the images.

### Locally (with Python)
1. Install the dependencies as mentioned above.
2. Run the Python script:
   ```bash
   python kannada_handwritten_text_search.py
3. Follow the prompts to upload and search in Kannada handwritten documents.



# Example Workflow:
1. Upload a Kannada handwritten document (PDF format).
2. Index the document, which extracts text from each page.
3. Search for specific phrases in the document.
4. View the highlighted results in the extracted text.




# Dependencies
pdf2image: Converts PDF pages into images.
opencv-python-headless: For image processing.
numpy: For numerical computations.
scipy: For spatial distance computations (optional).
pytesseract: Python wrapper for Tesseract OCR.
poppler-utils: Required for converting PDFs to images.
tesseract-ocr-kan: Kannada language OCR for Tesseract.



# OCR Language
The default OCR language is set to Kannada (kan). If you wish to work with other languages, 

adjust the OCR_LANGUAGE variable accordingly:
OCR_LANGUAGE = 'kan'  # Kannada Language Code



# How It Works:
1. Preprocess Image: Convert PDF pages into grayscale and binarized images for better OCR results.
2. Extract Text: Use Tesseract to extract handwritten Kannada text from each page.
3. Search for Phrase: Search through the extracted text to locate the specific phrase.
4. Highlight Phrase: Draw bounding boxes around the found phrases in the document image and display them.


# Limitations
1. Accuracy of text extraction may vary depending on the quality of the scanned document and handwriting clarity.
2. Only supports Kannada language for OCR in the current version.


# License
This project is licensed under the MIT License. See the LICENSE file for details.

# Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.

# Acknowledgments
Tesseract OCR - An open-source OCR engine.
Google Colab - For providing free cloud-based environments.



Let me know if you need further adjustments!
