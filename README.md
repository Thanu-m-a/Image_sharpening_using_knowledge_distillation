# Image Sharpening using Knowledge Distillation

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
| ![Input](results/input_sample.jpg) | ![Output](results/output_sharp.jpg) |

---

## References

- ResNet50: [https://arxiv.org/abs/2108.10257](https://medium.com/@nitishkundu1993/exploring-resnet50-an-in-depth-look-at-the-model-architecture-and-code-implementation-d8d8fa67e46f)
- BSDS500 Dataset: https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/

---

## License

MIT License
