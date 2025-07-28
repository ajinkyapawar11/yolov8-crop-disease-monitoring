# YOLOv8 Plant Disease Detection

## Overview
This project uses the YOLOv8 object detection model to identify leaf diseases in spinach, lettuce, and bok choy using CCTV imagery. It demonstrates a pilot implementation for smart greenhouse monitoring, with applications in agricultural automation and plant health assessment.

## Features
- Real-time detection using Ultralytics YOLOv8
- Focus on spinach, lettuce, and bok choy diseases
- Pilot project built using Roboflow dataset
- Evaluation using mAP metrics for performance tracking
- Supports inference on new images

## Dataset
The dataset was sourced from [Roboflow](https://universe.roboflow.com/hydromac/bok-choy-lettuce-spinach-diseased), containing labeled images for:
- Bok-Choy-Diseased
- Lettuce-Diseased
- Spinach-Diseased

## Getting Started

1. Clone the repository.
2. Open the notebook in [Google Colab](https://colab.research.google.com/).
3. Upload the dataset ZIP file.
4. Install dependencies using `!pip install ultralytics`.
5. Train the model using YOLOv8.
6. Perform validation and run inference on test images.

## Results
- Achieved **mAP@0.5: 0.864**
- Achieved **mAP@0.5:0.95: 0.571**
- YOLOv8n model trained with high accuracy on validation data.

## Sample Inference
Results saved in `/runs/detect/trainXX/` folders.
To test with a custom image:
```python
results = model.predict(source="your_image.jpg", save=True)
```

## License
This project is licensed under the MIT License.

## Author
Ajinkya Pawar
