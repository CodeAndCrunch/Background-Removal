# Background Removal Web Application

## Overview

The **Background Removal Web Application** is a user-friendly tool built with **Streamlit** that allows users to upload images and remove backgrounds easily. This application utilizes **image processing techniques** and an **API** to perform background removal based on user-selected coordinates. It provides an intuitive interface for users in various industries such as e-commerce, content creation, and design, helping them extract foreground objects or people from images.

## Features

* **Image Upload**: Upload images in **JPEG**, **JPG**, or **PNG** formats.
* **Interactive Image Handling**: Click on the image to select coordinates for background removal.
* **Background Removal**: Send the image and coordinates to an external API for background processing.
* **Original Image View**: Toggle between the **original** image and the processed image with background removed.
* **Customizable Background**: Set a custom background image for the Streamlit app.

## Technology Stack

* **Streamlit**: Framework for building the web interface.
* **OpenCV (cv2)**: Image processing library used for image manipulation (resizing, encoding, decoding, and background removal).
* **Pillow (PIL)**: Library used for opening, converting, and resizing images.
* **Requests**: For making HTTP requests to an external API for background removal.
* **Base64**: For encoding and decoding image data.
* **Numpy**: Used for array manipulation, particularly when working with pixel data.

## Installation

### Prerequisites

Before running the application, ensure that you have the following installed on your machine:

* Python 3.6 or later
* `pip` (Python package manager)

### Install Dependencies

Clone the repository and install the required libraries by running the following commands:

```bash
git clone https://github.com/your-repository/background-removal-app.git
cd background-removal-app
pip install -r requirements.txt
```

### External API Integration

You will need to provide an external API endpoint for the **background removal** functionality. In the script, this is currently set as `None`:

```python
api_endpoint = None  # Set this to the URL of the background removal API
```

Ensure that you replace `None` with a valid API endpoint that processes images and removes backgrounds.

### Run the Application

To start the Streamlit application, run the following command:

```bash
streamlit run app.py
```

This will launch the app in your default web browser.

## Usage

1. **Upload an Image**: Select an image (JPEG, PNG, JPG) from your local machine.
2. **Select Coordinates**: Click anywhere on the uploaded image to select a region for background removal.
3. **Remove Background**: Press the **"Remove Background"** button to send the image and selected coordinates to the background removal API.
4. **View Results**: The processed image with the background removed will be displayed. You can toggle between the **original** and **processed** images.
5. **Download Image**: After the background is removed, you can download the processed image with a transparent background.

## Customization

### Set Custom Background Image

The app allows you to customize the background of the interface. Replace the `bg.jpg` image file in the root directory with your preferred image.

```bash
./bg.jpg  # Replace with your custom background image
```

## Future Enhancements

* **Machine Learning Integration**: Implement automatic foreground detection to eliminate the need for manual coordinate selection.
* **Mobile Version**: Develop a mobile app for background removal on the go.
* **Cloud Storage Integration**: Store and manage processed images on cloud storage for better scalability and accessibility.
* **Advanced Image Editing**: Additional features like cropping, rotating, and adding text to images.

## Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. You can also report issues or suggest features by opening an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

* **Streamlit**: For creating an easy-to-use framework for building interactive web applications.
* **OpenCV**: For providing powerful image processing tools.
* **Requests**: For simplifying the HTTP requests to the external API.

---

Thank you for using the **Background Removal Web Application**! Feel free to reach out with any questions or suggestions.
