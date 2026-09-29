# Python Data Preparation

Jupyter notebooks with hands-on exercises on preparing structured data (tables),
images and text with Python.

## Exercises

| Notebook | Content |
|---|---|
| [advanced_data_preparation_apartment_data.ipynb](advanced_data_preparation_apartment_data.ipynb) | Worked example with scraped rental apartment data from Zurich. Covers regex extraction, handling missing and duplicated values, string manipulation, discretization, one-hot encoding, scaling, standardization, transformations (log, sqrt, Box-Cox), merging with geocoded and municipality data, sorting, reshaping (`stack`, `melt`) and pivot tables. |
| [advanced_data_preparation_car_data.ipynb](advanced_data_preparation_car_data.ipynb) | **Exercise:** apply the same steps to scraped car listings from AutoScout24. |
| [advanced_data_preparation_car_data_solution.ipynb](advanced_data_preparation_car_data_solution.ipynb) | Solution to the car data exercise. |
| [image_processing_with_opencv.ipynb](image_processing_with_opencv.ipynb) | Basic image processing with OpenCV: grayscale conversion, resizing, rotating, blurring and edge detection. |
| [natural_language_processing_spacy.ipynb](natural_language_processing_spacy.ipynb) | NLP basics with spaCy: tokenization, part-of-speech tagging, named entity recognition, dependency parsing and visualization with `displacy`. |
| [optical_character_recognition_pytesseract.ipynb](optical_character_recognition_pytesseract.ipynb) | OCR on a restaurant receipt with pytesseract: image preprocessing, text bounding boxes, template matching and saving the extracted text to a file. |

All input data is in the [Data/](Data/) folder.

## Setup

The easiest way is to open the repository in the provided dev container
([.devcontainer/devcontainer.json](.devcontainer/devcontainer.json)), for example in
GitHub Codespaces. It installs all Python packages and Tesseract OCR automatically.

To set it up manually (Python 3.11):

```bash
pip install -r requirements.txt

# Tesseract OCR engine with the German language pack (needed for the OCR notebook)
sudo apt-get install -y tesseract-ocr tesseract-ocr-deu
```

The spaCy notebook downloads the `en_core_web_sm` language model the first
time you run it.
