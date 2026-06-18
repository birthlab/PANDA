
# [IMAG] PANDA: Patch-based Unsupervised Deep Learning for Brain Anomaly Detection via Age Prediction in Fetal MRI

*Imaging Neuroscience*

---

### 🎯 **Multi-Disease Fetal Brain Anomaly Detection Using Brain Age Prediction: A Patch-based Deep Learning Framework**

<p align="center">
  <img src="Figure 1.png" width="85%">
</p>

---

## 📦 Download pretrained model

👉 [Click here](https://drive.google.com/file/d/1al1h63eVkVSexq1j77lpTFEY_zyYgfzt/view?usp=sharing)

---

## 🚀 Usage

### 1️⃣ Data Preprocessing before training or inference

Run

```bash
python preprocess.py
```

with an *nii.gz brain and an output path.*

---

### 2️⃣ Inference

Example command:

```bash
python inference_one_brain.py /path/to/brain_patches 215 --model best_model.pt
```

The path here is the output path of step 1. The gestational age is measured in **DAYS** here.

---

### 3️⃣ Train your own age prediction model

Prepare an xlsx file with two columns: ID and Age, then run

```bash
python train.py
```

---

## 🧩 Visualization of Patch-wise Prediction

<p align="center">
  <img src="Figure 3.png" width="85%">
</p>

---


## 🙏 Acknowledgements

### We gratefully acknowledge the contributions of the following repos to our work.

1. https://github.com/gift-surg/NiftyMIC
2. https://github.com/ha-ha-ha-han/UKBiobank_deep_pretrain

---

## 📖 Citation

If you find this work useful for your research, please consider citing our paper:

```bibtex
@article{10.1162/IMAG.a.1293,
    author = {Hao, Yingqi and Liu, Mingxuan and Zhu, Juncheng and Yang, Hongjia and Li, Haoxiang and Kang, Min and Song, Yan and Lai, Hua and Zhou, Xiaoling and Ning, Gang and Liao, Yi and Qu, Haibo and Tian, Qiyuan},
    title = {PANDA: Patch-based Unsupervised Deep Learning for Brain Anomaly Detection via Age Prediction in Fetal MRI},
    journal = {Imaging Neuroscience},
    year = {2026},
    month = {06},
    issn = {2837-6056},
    doi = {10.1162/IMAG.a.1293},
    url = {https://doi.org/10.1162/IMAG.a.1293},
    eprint = {https://direct.mit.edu/imag/article-pdf/doi/10.1162/IMAG.a.1293/2607082/imag.a.1293.pdf},
}
