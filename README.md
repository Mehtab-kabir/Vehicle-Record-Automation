# Automatic License Plate Detection and Recognition

This project implements an automated system for detecting and recognizing license plates from video footage. It uses the YOLO (You Only Look Once) model for object detection and EasyOCR for extracting text from detected license plates. The system is designed to process video frames, annotate detected license plates, and include timestamp information, making it ideal for traffic monitoring and surveillance applications.

---

## Features

- **Real-time License Plate Detection**: Utilizes a pre-trained YOLO model to detect license plates in video frames.
- **OCR for Text Recognition**: Extracts text from detected license plates using EasyOCR.
- **Timestamp Extraction**: Uses OCR to read timestamps embedded in the video frames.
- **Annotated Outputs**: Annotates video frames with detected license plate numbers and corresponding timestamps.
- **Scalable Implementation**: Easily extendable for different types of input videos and datasets.

---

## Requirements

- Python 3.7+
- YOLO (pre-trained model weights for license plate detection)
- EasyOCR
- OpenCV
- Google Colab (for running the project, optional)

Install the required dependencies using:
```bash
pip install -r requirements.txt
```

---

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/license-plate-detection.git
   cd license-plate-detection
   ```

2. Place your YOLO model weights in the specified directory (update the path in the script if needed).

3. Replace the `video_path` variable with the path to your input video file:
   ```python
   video_path = '/path/to/your/video.mp4'
   ```

4. Run the script to process the video:
   ```bash
   python license_plate_detection.py
   ```

---

## Usage

1. **Input Video**: Provide a video file with vehicles and visible license plates.
2. **Processing**: The script will detect license plates, extract their text, and overlay the results along with timestamps on the video frames.
3. **Output**: Annotated frames can be displayed or saved for further analysis.

---

## Example Output

For a given video frame:
- **Detected License Plate**: ABC1234
- **Extracted Timestamp**: 10:15:23

The annotated frame includes:
- Bounding boxes around the license plates.
- Text annotations with the license plate numbers.
- Timestamp overlay.

---

## Technologies Used

- **YOLO**: For object detection.
- **EasyOCR**: For optical character recognition of license plates.
- **OpenCV**: For video frame processing and visualization.
- **Python**: Core programming language for the implementation.

---

## Future Enhancements

- Support for multiple languages in license plate text.
- Integration with a database for storing and querying recognized plates.
- Improved accuracy through fine-tuned YOLO models.
- Support for live video streams.

---

## Contributing

Contributions are welcome! Please fork the repository, create a feature branch, and submit a pull request with your changes.

---
