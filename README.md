# Image Sharpening using Knowledge Distillation

This project explores **image sharpening** using a **teacher-student framework** through **knowledge distillation (KD)**. This project demonstrates how to sharpen low-resolution or blurred images using a lightweight **student model** trained with **knowledge distillation** pretrained high-capacity model ResNet-50 from a more powerful **teacher model**. The training is guided by structural similarity (SSIM), Peak Signal-to-Noise Ratio (PSNR), mean squared error (MSE), and output matching with the teacher.

---

## Overview

- **Teacher Model**: ResNet-50
- **Student Model**: Lightweight CNN 
- **Task**: Learn sharpening filters via KD
- **Dataset**: BSDS500
- **Metric**: Structural Similarity Index (SSIM), Peak Signal-to-Noise Ratio (PSNR)

---

## Results

| Metric | Value |
|--------|-------|
| SSIM   | ~86.24 |
| PSNR   | ~29.2 |
| FPS Benchmark | ~9.88 |

---

## How to Run

1. Clone this repository:

```bash
git clone https://github.com/yourusername/image-sharpening-kd.git
cd image-sharpening-kd
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the notebook:

```bash
jupyter notebook image_sharpening_kd.ipynb
```

---

## Sample Results

| Input | Output (Sharpened) |
|-------|--------------------|
| <img width="200" height="200" alt="Image" src="https://github.com/user-attachments/assets/87ca8034-3810-4e9c-9ddc-c162a2ddedc7" /> | <img width="190" height="125" alt="Image" src="https://github.com/user-attachments/assets/59fbd0fc-5c00-40dc-b32f-5f51c2b508f0" />

---

## References

- ResNet50: [https://arxiv.org/abs/2108.10257](https://medium.com/@nitishkundu1993/exploring-resnet50-an-in-depth-look-at-the-model-architecture-and-code-implementation-d8d8fa67e46f)
- BSDS500 Dataset: https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/

---

