# Yamaha Parts Detection with DETR

This project uses **Meta AI's DETR (DEtection TRansformer)** to detect and classify Yamaha motorcycle parts from real-world images. The model was trained on a custom dataset annotated in COCO format and visualized using the `supervision` library.

---

## 🔍 Project Overview

- 🎯 **Objective**: Automatically detect and label different Yamaha motorbike components in images.
- 🧠 **Model**: DETR by Meta AI, with a ResNet backbone.
- ⚙️ **Frameworks**: PyTorch, Hugging Face Transformers, Supervision, Roboflow.

---

## 🧪 Example Results

Below are examples of ground truth annotations and model predictions:

| Ground Truth | DETR Prediction |
|--------------|-----------------|
| <img width="1252" height="1252" alt="imagen123" src="https://github.com/user-attachments/assets/97dbfbce-1f0c-4589-bc64-91a0ca6dc888" /> | <img width="1252" height="1252" alt="pred111" src="https://github.com/user-attachments/assets/6f1c673c-dd26-4f18-a913-3ac626fdaee9" /> |
| <img width="1252" height="1252" alt="345" src="https://github.com/user-attachments/assets/875c3699-cf69-4ced-b8e5-d3c8dfbb3db7" /> | <img width="1252" height="1252" alt="346" src="https://github.com/user-attachments/assets/cc218e57-1c99-42d3-9e58-3606198938d2" /> |

---

## 📈 Evaluation Results

The model was evaluated using COCO metrics and achieved the following:

- **mAP@[0.5:0.95]**: `0.768`
- **AP@0.5**: `0.953`
- **AP@0.75**: `0.922`
- **AR@100 (all sizes)**: `0.796`
- **AP for large objects**: `0.781`
- **AP for medium objects**: `0.434`
- **AP for small objects**: `N/A`

These results show that DETR performs exceptionally well on Yamaha motorbike parts, especially for large and well-defined components.
