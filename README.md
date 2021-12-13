# tugaspraktikum_ML5

# OVERVIEW JURNAL
Skin Lesion Analysis Toward Melanoma Detection: A Challenge at the 2017 International Symposium on Biomedical Imaging (ISBI), Hosted by the International Skin Imaging Collaboration (ISIC), 
- dataset yang digunakan " http://challenge2017.isic-archive.com/ " didalamnya sudah terdapat testing, training, validation
- Lesion Segmentation, Dermoscopic Feature Classification, Disease Classification

# OVERVIEW DATASET
-https://www.kaggle.com/wanderdust/skin-lesion-analysis-toward-melanoma-detection
![image](https://user-images.githubusercontent.com/64590037/143798029-dd668b1a-2f0f-4258-9cf0-69d1aa9f00c1.png)
- terdapat 3 kelas
- tranin : melanoma (374 images), nevus (1372 images), seborrheic_keratosis (254 images)
- test : melanoma (117 images), nevus (393 images), seborrheic_keratosis (90 images)
- valid : melanoma (30 images), (78 images), seborrheic_keratosis (42 images)
- Data dibagi menjadi:

    data pelatihan (2000 gambar)
    dataset validasi (150 gambar)
    kumpulan data uji (600 gambar)

- spillting (80, 19, 1)
- keseluruhan data adalah 2570


# PRE-PROCESSING
- size (128,128)
- horizontal flip (True)
- suffle (True)
- batch_size (32)
- class_mode (categorical)
- color_mode (rgb)

![Screenshot (292)](https://user-images.githubusercontent.com/64590037/145890151-6d8d3f42-e266-4a98-97c2-d6f1afa5afc5.png)

# MODEL YANG DIGUNAKAN
-MODEL 1
- menggunakan pretrained model (MobileNetV2, DenseNet121)
- untuk melakukan balencing dataset, tidak memungkinkan karena dataset saya menggunakan flow for directory, kecuali menggunakan flow saja
![Screenshot (293)](https://user-images.githubusercontent.com/64590037/145890273-ef08a6e1-bc65-4a56-af78-af8f253f3b54.png)

![Screenshot (294)](https://user-images.githubusercontent.com/64590037/145890441-996c3ec8-9096-4c2e-8090-be774686171a.png)

![Screenshot (295)](https://user-images.githubusercontent.com/64590037/145890473-c6dd7eda-f208-4919-9d83-844b20d1e686.png)

