# YOLOv9 for Surveillance

## Introduction
YOLOv9 (You Only Look Once, Version 9) is an advanced object detection model designed for high-speed and accurate detections. This implementation demonstrates the potential of YOLOv9 in surveillance systems, leveraging its robust detection capabilities to analyze video feeds in real-time. The model has been trained using the IDD (Indian Driving Dataset) to detect various objects with precision.

## Key Features
- **High Accuracy**: Achieved 92% accuracy on the IDD dataset, validated against public benchmarks.
- **Real-Time Performance**: Optimized for speed, making it ideal for live surveillance applications.
- **Versatile**: Capable of detecting multiple object classes, customizable for specific surveillance needs.

## Dataset
We utilized the **IDD (Indian Driving Dataset)** for training the model. The IDD dataset is well-suited for real-world scenarios, especially in diverse and complex environments. It provides a comprehensive set of labeled images, allowing the model to generalize effectively.

Dataset and associated Jupyter Notebook files are available for download if required: [Google Drive Link](https://drive.google.com/drive/folders/1S-OHaFSG8WHfYZhGESi3G4b32KD7DC-4?usp=sharing).

## Model Performance
- **Training Accuracy**: 92%
- **Validation**: Tested on public benchmarks with consistent performance.
- **Use Case**: Demonstrated efficacy in surveillance systems for real-time object detection and monitoring.

## Requirements
To run this model, ensure the following dependencies are installed:

```bash
pip install -r requirements.txt
```

### Key Libraries:
- Python 3.8+
- PyTorch 1.9+
- OpenCV
- YOLOv9 (custom implementation)

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/Dharunraagav/Yolov9.git
   ```
2. Navigate to the project directory:
   ```bash
   cd yolov9
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the model on sample data:
   ```bash
   python detect.py --source ./data/sample_video.mp4
   ```

## Training
To train the YOLOv9 model on a custom dataset:
1. Prepare the dataset in YOLO format.
2. Update the configuration file with the dataset path.
3. Start training:
   ```bash
   python train.py --data ./data/idd.yaml --cfg ./models/yolov9.yaml --epochs 100
   ```

## Evaluation
Evaluate the model on a test dataset:
```bash
python val.py --data ./data/idd.yaml --weights ./weights/best.pt
```

## Acknowledgments
- The creators of the **IDD Dataset** for providing an extensive labeled dataset.
- The open-source community for contributions to YOLOv9 and PyTorch.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contact
For any queries or contributions, please contact [dharunraagav@gmail.com].

