# 至SRGAN官方Git下載文件
[點我前往](https://github.com/tensorlayer/srgan)

而資料最主要的會有 **config.py**、**srgan.py**、**train.py**、**vgg.py**
![image](https://user-images.githubusercontent.com/46515944/198824271-28d864d7-67d0-4684-bdab-8d95cd1bcc0d.png)


# 下載預VGG-19訓練檔
將檔案 **vgg19.npy** 放在 srgan/model 下(請另創model資料夾)
或[點這下載](https://drive.google.com/file/d/1CLw6Cn3yNI1N15HyX99_Zy9QnDcgP3q7/view?usp=sharing)

![image](https://user-images.githubusercontent.com/46515944/198824361-873a97d0-4d8e-4ebe-a50a-ac9976237c8a.png)

# 訓練自己的圖片
除了train與valid兩資料夾外，還需要建立縮小4倍，低解析度的優
結構如下

    srgan/
        └── config.py
        └── srgan.py
        └── train.py
        └── vgg.py
        └── model
              └── vgg19.npy
        └── DIV2K
              └── DIV2K_train_HR
              ├── DIV2K_train_LR_bicubic
              ├── DIV2K_valid_HR
              └── DIV2K_valid_LR_bicubic
