![Input](https://github.com/user-attachments/assets/ce262cfd-a41f-4867-81ec-f2b737fb52d0)# Image Sharpening using Knowledge Distillation

This project explores **image sharpening** using a **teacher-student framework** through **knowledge distillation (KD)**. The goal is to enhance image clarity by learning from a pretrained high-capacity model (e.g., SwinIR or ResNet-50) and distilling the sharpening knowledge into a lightweight student model.

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
| SSIM   | ~0.85 |
| PSNR   | ~29.2 |

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
| ![Image](https://github.com/user-attachments/assets/edf6ff88-6a9d-449b-98f7-4d87cd1bd32d) | ![Output](results/output_sharp.jpg) | <img width="256" height="256" alt="Image" src="https://github.com/user-attachments/assets/59fbd0fc-5c00-40dc-b32f-5f51c2b508f0" />

---

## References

- ResNet50: [https://arxiv.org/abs/2108.10257](https://medium.com/@nitishkundu1993/exploring-resnet50-an-in-depth-look-at-the-model-architecture-and-code-implementation-d8d8fa67e46f)
- BSDS500 Dataset: https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/

---

## License

MIT License
