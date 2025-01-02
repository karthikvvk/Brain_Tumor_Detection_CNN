# AI Tumor Detection and AI Pill Detector

## Overview
This repository includes a single AI-powered website built using **Streamlit** that combines two applications:

1. **AI Tumor Detection**: Detects brain tumors from medical images and provides detailed AI-generated diagnostic reports.
2. **AI Pill Detector**: Identifies pills based on uploaded images and provides detailed information, including name, usage, dosage, and purpose.

This website is designed to help patients understand complex medical images and products more easily.

---

## Features
### AI Tumor Detection
- Detects the presence of brain tumors from medical images.
- Generates a detailed diagnostic report.
- Provides insights into the tumor's type and characteristics.

### AI Pill Detector
- Identifies pills based on an image uploaded by the user.
- Extracts and displays the pill's name, dosage, and usage.
- Explains the pill's purpose and relevant precautions.

---

## Setup Instructions

### Prerequisites
Ensure you have Python installed (version 3.8 or later). Install the required libraries by following the steps below.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Sudharshana426/Brain_Tumor_Detection_CNN.git
   cd Brain_Tumor_Detection_CNN
   ```

2. Install the required Python packages:
   ```bash
   pip install google-generativeai rapidfuzz requests beautifulsoup4 easyocr opencv-python textblob streamlit pandas numpy matplotlib seaborn
   ```

---

## Usage

### Running the Website
1. Run the Streamlit application:
   ```bash
   streamlit run app.py
   ```
2. Access the website in your browser to:
   - Upload medical images for tumor detection and receive a detailed diagnostic report.
   - Upload pill images to get detailed information about the pill.

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

## Libraries Used
- **google-generativeai**: For AI-based diagnostic reporting.
- **rapidfuzz**: For string matching and comparison.
- **requests**: For making API calls.
- **beautifulsoup4**: For web scraping (if needed).
- **easyocr**: For optical character recognition in pill detection.
- **opencv-python**: For image processing.
- **textblob**: For text analysis and language processing.
- **streamlit**: For creating interactive web-based interfaces.
- **Pandas and NumPy**: For data manipulation and analysis.
- **Matplotlib and Seaborn**: For visualization.

---

## Contributions
Contributions are welcome! Feel free to fork this repository, make enhancements, and submit a pull request.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact
For any questions or issues, please create an issue in this repository or contact the author via GitHub.
