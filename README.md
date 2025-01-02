# AI Brain Tumor Detection and AI Pill Detector

## Overview
This repository includes a single AI-powered website built using **Streamlit** that combines two applications:

1. **AI Tumor Detection**: Detects brain tumors from medical images and provides detailed AI-generated diagnostic reports.
2. **AI Pill Detector**: Identifies pills based on uploaded images and provides detailed information, including name, usage, dosage, and purpose.

This website is designed to help patients understand complex medical images and products more easily.

---

## Features
### AI Tumor Detection
- Detects four types of brain conditions from MRI scans: Glioma, Meningioma, Pituitary, and No Tumor.
- Utilizes saliency maps to provide visual cues highlighting tumor regions in MRI scans.
- Provides a detailed diagnostic report for further medical consultation.

### AI Pill Detector
- Identifies pills based on an image uploaded by the user.
- Extracts and displays the pill's name, dosage, and usage.
- Explains the pill's purpose and relevant precautions.

**Check out our demo video
https://drive.google.com/file/d/1GDIUwd6NJ0ctm8fn1dJILZ72TJ7x8vT2/view?usp=drive_link

For detailed Knowledge check out the Project Report
https://drive.google.com/file/d/1ex1dqJswvWu7crkWTsySBZs1pWQNsIoB/view?usp=drive_link**
---

## Setup Instructions

### 1. Backend Setup

#### **1.1 Install Python**
Ensure Python 3.8 or later is installed. You can download it from [https://www.python.org/downloads/](https://www.python.org/downloads/).

#### **1.2 Create and Activate a Virtual Environment**
```bash
python3 -m venv venv
source venv/bin/activate  # For Linux/Mac
venv\Scripts\activate     # For Windows
```

#### **1.3 Install Required Python Libraries**
Install dependencies from the `requirements.txt` file:
```bash
pip install -r requirements.txt
```

#### **1.4 Install Additional Libraries**
If `requirements.txt` does not cover all, manually install:
```bash
pip install easyocr opencv-python-headless requests beautifulsoup4 textblob rapidfuzz google-generativeai pandas numpy matplotlib seaborn
```

#### **1.5 Set Up API Key for Generative AI**
1. Replace the `api_key` in `ai.py` with your valid API key for the **Google Generative AI** platform.
2. Create a `.env` file to store sensitive information securely:
   ```env
   GOOGLE_API_KEY=your_google_api_key
   ```

---

### 2. Run the Project

#### **2.1 Start the Streamlit Application**
Run the Streamlit application directly:
```bash
streamlit run app.py
```
The application will open in your browser.

#### **2.2 Use the Application**
1. Upload an MRI scan to the Tumor Detection section.
   - The model will process the image and classify it into one of the four categories (Glioma, Meningioma, Pituitary, or No Tumor).
   - The saliency map will highlight the tumor region if present.
2. Upload an image of a pill to the Pill Detector section.
   - The application will analyze the image and provide details like pill name, dosage, and purpose.

---

### 3. Notes
- Ensure that the **uploaded MRI scans and pill images** meet the supported formats (e.g., JPG, PNG).
- Store large datasets (like weights or drug lists) in a separate file or database for scalability.
- Use Google Colab for GPU-enabled infrastructure to improve model performance during testing or training.

---

### Dependencies
- **Python Libraries**: EasyOCR, OpenCV, BeautifulSoup, Requests, TextBlob, RapidFuzz, Google Generative AI SDK, Pandas, NumPy, Matplotlib, Seaborn.
- **Frameworks**: TensorFlow for deep learning and Streamlit for the web application.

---

### Troubleshooting
- **EasyOCR Errors**: Install language-specific OCR model files if `easyocr.Reader` raises errors.
- **Google API Issues**: Verify the API key validity and usage quotas.
- **Streamlit Issues**: Ensure all required libraries are installed and the correct Python version is used.

---

## File Structure
```
Brain_Tumor_Detection_CNN/
|-- app.py                    # Streamlit application script
|-- tumor_detection.py         # Script for tumor detection
|-- pill_detector.py           # Script for pill detection
|-- models/                    # Pre-trained models for both applications
|-- requirements.txt           # Dependencies
|-- data/                      # Placeholder for input data
|-- outputs/                   # Placeholder for results and reports
|-- README.md                  # Documentation
```

---

## Contributions
Contributions are welcome! Feel free to fork this repository, make enhancements, and submit a pull request.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---


## Contact
For any questions or issues, please create an issue in this repository or contact the author via GitHub.
