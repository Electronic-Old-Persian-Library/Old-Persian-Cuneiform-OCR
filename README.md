## The aim of this repository is creating an OCR model (convert image to text) for Old Persian Cuneiform 

This repository is inspired from [eBL project](https://github.com/ElectronicBabylonianLiterature) and is a part of [
Electronic Old Persian Library](https://github.com/Electronic-Old-Persian-Library) organization.

eBL has developed models for Babylonian cuneiform but I am going to develop my models for Old Persian cuneiform. 


## Three OCR models are developed in this repository:
- ``` yolo_cnn_old_persian ```
- ``` tessearct_old_persian ```
- ``` easyocr_old_persian ```
## Current status of these 3 OCR models:
- ``` yolo_cnn_old_persian ``` : is not completed yet.
-  ``` tessearct_old_persian ``` is completed.
-  ``` easyocr_old_persian ``` is completed but needs more optimization and real data.

Melanee: Since I was looking for an OCR model for Old Persian language, I have not implemented image pre-processing for my models yet and they work on just black and white images. You can use [custom images](https://github.com/Melanee-Melanee/Old-Persian-Cuneiform-OCR/tree/master/other/custom%20images) to use my OCR models.

## easyocr_old_persian

This model is still under developing and is based on [EasyOCR](https://github.com/JaidedAI/EasyOCR/blob/master/custom_model.md) repository for a custum model. 
If you see any error please check [issues](https://github.com/JaidedAI/EasyOCR/issues)

Trainer notebook:

https://github.com/Melanee-Melanee/Old-Persian-Cuneiform-OCR/blob/master/easyocr_old_persian/trainer_easyocr_old_persian.ipynb

Using saved model:

https://github.com/Melanee-Melanee/Old-Persian-Cuneiform-OCR/blob/master/easyocr_old_persian/model_easyocr.ipynb

To use saved model please create the ```root``` of your machine like below structure and replace ```custum_example.pth```, ```custom_example.py``` and ```custom_example.yaml``` files there. For more comprehension please watch this tutorial on [youtube](https://www.youtube.com/watch?v=-j3TbyceShY).

/root/

     /EasyOCR/
           /model/
               custum_example.pth
           /user_network/
               custom_example.py
               custom_example.yaml



## tessearct_old_persian:

https://github.com/Melanee-Melanee/Old-Persian-Cuneiform-OCR/blob/main/Tesseract_Old_Persian_OCR.ipynb

Please replace ```myLang.traineddata``` file in this directory: `/usr/share/tesseract-ocr/4.00/tessdata`

This tesseract pre-trained OCR model deciphers Old Persian cuneiform to English transcription and is developed by [S. Muhammad Hossein Mousavi](https://github.com/SeyedMuhammadHosseinMousavi/Extracting-Old-Persian-Cuneiform/tree/main
). [Tesseract](https://github.com/tesseract-ocr/tesseract) is one of the most powerful OCR models in the world.


An example: 

The last 12 lines of the great Darius's inscription in Persepolis, [DPd inscription](https://www.livius.org/sources/content/achaemenid-royal-inscriptions/dpd/):

Input:

![darius2](https://github.com/Melanee-Melanee/Old-Persian-Cuneiform-OCR/assets/74653444/fc8f2a4c-b8b4-4b46-97e3-c87d506fd6fd)



Output:

Zittiy ; iaryvuS ; xrSayZiy;

mnc;aurmzia;upstam; rlauv;

hia ; ViZiriS ; rgiriS ; uta;

im am ; i h yaum ; au lm z i a ;

pitTucs;hca;hinaya; hca;

QuSiyala ; hca;iruga;ariy;

imam ;ihyaum;ma; ajMiya; ait;

aim ;yanm;jDiyaMiy;

aitmiy ; iiaTuv

## At the next step, you can translate that Old Persian transcription to modern languages by [Chat-GPT](https://chatgpt.com/):

Translate to Modern Persian:




این منم داریوش شاهنشاه؛
به لطف اهورامزدا، من این را بنا کردم؛
من این امپراتوری را بنیان نهادم و آن را نیرومند ساختم.
باشد که اهورامزدا من و پادشاهی مرا محافظت کند؛
باشد که برای همیشه پایدار بماند؛
و باشد که از دروغ در امان باشد؛
این است آنچه من انجام دادم؛

این است آنچه من می‌گویم.

Translate to Modern English:

“This is me, Dariush king; By the grace of Ahura Mazda, I have built this; I founded this empire and made it strong. May Ahuramazda protect me and my kingdom; may it last forever; and it would be safe from lies; that is what I did;
That is what I am saying.”

## Article

I wrote an [article](https://www.researchgate.net/publication/382528886_Translating_Old_Persian_cuneiform_by_artificial_intelligence_AI) as a tiny report for what I have done for this project till now.

## Notice

This repository is still under developing. For contributing contact me by email: melaneepython@gmail.com 

To create pull requests for this repository please choose just these branches: issue, refactor and feature.


