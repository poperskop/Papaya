# Dataset Overview
Guava (Psidium guajava) is a key crop in South Asia, especially in Bangladesh. Rich in vitamin C and fiber, it supports regional economies and nutrition. Unfortunately, guava production is threatened by diseases that reduce yields. This dataset is designed to aid the development of machine learning models for early disease detection in guava fruit, helping to protect harvests and reduce economic losses.

## Dataset Summary
This dataset includes 473 annotated images of guava fruits, categorized into three classes. Images underwent preprocessing steps such as unsharp masking and CLAHE. The preprocessed images are augmented to increase in number to 3,784 image data. The three classes are:

- Anthracnose
- Fruit Flies
- Healthy fruits
Images were collected from guava orchards in Rajshahi and Pabna, Bangladesh, during the fruit-ripening season in July when disease vulnerability is highest. A plant pathologist verified the images for accuracy in classification. Each image was preprocessed to a consistent size of 512 x 512 pixels in RGB format, suitable for deep learning and image processing applications.

## My solution
For model i used (WinKawaks/vit-tiny-patch16-224)[https://huggingface.co/WinKawaks/vit-tiny-patch16-224] as backbone and classification head on top of it.

metrics values:
```
Training Loss :		 0.164200
Validation Loss:		0.132089
 Anthracnose/precision:		0.990637
 Anthracnose/recall :		1.000000
Anthracnose/f1-score :		0.995296
Fruit Fly/precision :		0.929577
Fruit Fly/recall :		1.000000
Fruit Fly/f1-score :		0.963504
Healthy Guava/precision :		1.000000
Healthy Guava/recall :		0.840426
Healthy Guava/f1-score :		0.913295
Accuracy :		0.980132
Macro avg/precision:		0.973405
 Macro avg/recall:		0.946809
 Macro avg/f1-score:		0.957365
 Weighted avg/precision:		0.981127
 Weighted avg/recall :		0.980132
Weighted avg/f1-score:		0.979528
```

## Dataset origin
```
Amin, Md Al; Mahmud, Md Iqbal; Rahman, Asadullah Bin; Parvin, Mst Aktarina; Mamun, Md Abdulla Al (2024), “Guava Fruit Disease Dataset”, Mendeley Data, V1, doi: 10.17632/bkdkc4n835.1
```
