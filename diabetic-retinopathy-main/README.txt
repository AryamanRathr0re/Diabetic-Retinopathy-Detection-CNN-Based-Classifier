# Diabetic Retinopathy Detection System

A modern web application that uses deep learning to detect and classify diabetic retinopathy from retinal images.

## 🚀 Quick Setup Guide

### Prerequisites

1. Python 3.10.x (recommended)
   - Download from: https://www.python.org/downloads/
   - ✅ Make sure to check "Add Python to PATH" during installation

2. Visual Studio Build Tools (required for some dependencies)
   - Download from: https://visualstudio.microsoft.com/visual-cpp-build-tools/
   - During installation, select "Desktop development with C++"

### Installation Steps

1. Clone or download this repository
   ```
   git clone <repository-url>
   cd diabetic-retinopathy-main
   ```

2. Set up a Python virtual environment (recommended)
   ```
   python -m venv venv
   ```

3. Activate the virtual environment
   - Windows:
     ```
     .\venv\Scripts\activate
     ```
   - Linux/Mac:
     ```
     source venv/bin/activate
     ```

4. Install required packages
   ```
   pip install -r requirements.txt
   ```

5. Configure the output directory
   - Open `diabetic_retinopathy/settings.py`
   - Locate the `STATIC_URL` setting
   - Update it to your local path:
     ```python
     STATIC_URL = 'YOUR_PROJECT_PATH/diabetic-retinopathy-main/diab_retina_app/output/'
     ```

6. Initialize the database
   ```
   python manage.py migrate
   ```

7. Start the development server
   ```
   python manage.py runserver
   ```

8. Access the application
   - Open your web browser
   - Go to: http://127.0.0.1:8000/

## 📝 Usage Instructions

1. Once the application is running, you'll see a modern interface for uploading retinal images
2. Click "Choose Image" to select a retinal image
3. Supported formats: JPG, PNG (Max size: 5MB)
4. After selecting an image, click "Analyze Image"
5. Wait for the analysis to complete
6. View the results showing:
   - Diagnosis
   - Confidence level

## 🔍 Test Images

- Sample test images are available in the `diab_retina_app/test` directory
- Use these for testing the system's functionality

## ⚠️ Troubleshooting

1. If Python is not recognized:
   - Make sure Python is added to PATH
   - Try using the full path to Python: `C:\Users\[YourUsername]\AppData\Local\Programs\Python\Python310\python.exe`

2. If pip install fails:
   - Make sure Visual Studio Build Tools are installed
   - Try updating pip: `python -m pip install --upgrade pip`
   - Install packages one by one if needed

3. If the server doesn't start:
   - Check if port 8000 is available
   - Try a different port: `python manage.py runserver 8080`

4. If images don't process:
   - Verify the STATIC_URL path is correct
   - Check file permissions in the output directory

## 🛠️ System Requirements

- Python 3.10.x
- 4GB RAM minimum (8GB recommended)
- Windows 10/11, Linux, or macOS
- Modern web browser (Chrome, Firefox, Edge recommended)

## 📋 Dependencies

Major packages used:
- Django 5.0.3
- TensorFlow 2.8.0
- NumPy 1.24.3
- Pillow (PIL) for image processing
- Other dependencies listed in requirements.txt

## 🤝 Support

For issues and questions:
- Check the troubleshooting section
- Submit an issue on the repository
- Contact the development team

---
Made with ❤️ for better healthcare diagnostics