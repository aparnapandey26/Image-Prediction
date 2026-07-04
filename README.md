# Image-Prediction
# Image Prediction API

## Project Description

This project is an Image Prediction API built using FastAPI and TensorFlow's pre-trained MobileNetV2 model.

Users can upload an image, and the API predicts the object present in the image along with the confidence score.

## Technologies Used

- Python
- FastAPI
- TensorFlow
- MobileNetV2
- Pillow
- NumPy
- Uvicorn

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Run the API

```bash
uvicorn app:app --reload
```

## Open Swagger UI

```
http://127.0.0.1:8000/docs
```

## API Endpoint

### GET /

Returns:

```json
{
  "message": "Image Prediction API is Running"
}
```

### POST /predict

Upload an image file.

Example Response:

```json
{
  "Prediction": "golden_retriever",
  "Confidence": 94.02
}
```

## Model Used

MobileNetV2 (Pre-trained on ImageNet)

## Author

Aparna Pandey
