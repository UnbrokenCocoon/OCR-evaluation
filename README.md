# OCR Accuracy Evaluation for Image-Based Text Extraction

This project is a practical, beginner-friendly guide for users with datasets of scanned images, archival documents, or photos of text who want to extract accurate text using OCR — no deep technical setup required.

All workflows run in **Google Colab**, so you don’t need to install anything locally.

---

##  What You’ll Learn / Do

- Test 4 OCR tools side by side: **Tesseract**, **EasyOCR**, **PaddleOCR**, and **Gemini**
- Improve accuracy with image preprocessing (grayscale, thresholding, shadow removal)
- See which tool performs best for your dataset
- Evaluate OCR output using **Word Error Rate (WER)** and **Character Error Rate (CER)**

---

## Try It Out (Colab Links)

| Notebook                        | Description                                  | Link                                                                 |
|----------------------------------|----------------------------------------------|----------------------------------------------------------------------|
| 🧪 `OCR_packages_comparison`     | Compare multiple OCR engines on one image    | [Open in Colab](https://colab.research.google.com/drive/1XZEeED3dpC1I8RFKbuBM8u_Fj3ubvlce?usp=sharing) |
| 📅 `Preprocessing_demo`          | Show impact of preprocessing visually        | [Open in Colab](https://colab.research.google.com/drive/19uHXxZeSgFFP2cyhGbLQU4MeBjq0wAcg?usp=sharing) |
| 🤖 `Gemini_error_solution`       | Fixing Gemini setup and API usage            | [Open in Colab](https://colab.research.google.com/drive/15y3SyS0RqmygtxHQT24ghG0L59gZjix8?usp=sharing) |
| 🔍 `LLM_OCR_comparison`          | Compare LLMs vs. OCR tools                   | [Open in Colab](https://colab.research.google.com/drive/1f-9GX1nC2egqaZxmCIdFMkNXifL9FchB?usp=sharing) |


Images should be placed in your Google Drive under `/OCR evaluation/Data/`

---


## Sample OCR + LLM Accuracy Table

| Engine           |   WER |   CER | LLM   |
|:-----------------|------:|------:|:------|
| Gemini 2-0 Flash |  0.04 |  0.02 | Yes   |
| Qwen3-235B-A22B  |  0.06 |  0.03 | Yes   |
| Deepseek-V3-R1   |  0.29 |  0.26 | Yes   |
| Chat GBT 4-o     |  0.58 |  0.45 | Yes   |
| Tesseract        |  0.69 |  0.43 | No    |
| PaddleOCR        |  0.79 |  0.76 | No    |
| EasyOCR          |  0.89 |  0.67 | No    |


---

## Who This Is For

This repo is ideal for:
-  Humanities & archive researchers with scanned documents
-  Social scientists or students digitising printed material
-  Anyone with a folder of photos who just wants to know:  
  *"Which OCR tool gives me the best results?"*

You don’t need to install Python, or understand OCR theory — everything runs in Google Colab.

---

## 📌 Notes

- Google Drive is used to store image data and outputs
- Preprocessing is optional, but highly recommended for historical or noisy images
- WER/CER comparisons use [`jiwer`](https://github.com/jitsi/jiwer) for reproducibility

---

## 👌 Credits

Built with:
- [EasyOCR](https://github.com/JaidedAI/EasyOCR)
- [Pytesseract](https://github.com/madmaze/pytesseract)
- [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)
- [Google Gemini](https://makersuite.google.com/)
- [`jiwer`](https://github.com/jitsi/jiwer) for WER/CER

---

📬 Feedback or questions? Feel free to open an issue or fork the repo.

