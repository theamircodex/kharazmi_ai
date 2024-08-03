# نکته قابل توجه : 
تاریخ گیتهاب هفتگی بروزرسانی میشود , آخرین تغییراتی که تغییرات سورس کد طرح SRCCODE.zip مربوط به 22 و 23 جولای بوده که معادل یکم و دوم مرداد است زمانی که سامانه جــــشــنوا_ره هنوز باز بوده و تغییرات مجاز بوده است. این نکته تاریخ گیتهاب را الان متوجه شدم (امروز 12 مرداد) و با نظر پشتبانی تصمیم گرفتم از طریق این فایل به اطلاع شما برسانم

سلام خدمت داوران گرامی لطفا فایل SRCCODE.zip را دانلود و استخراج کنید تمامی سورس کد ها داخل موجود است. منظور Download raw file


در هنگام دانلود اگر با ارور آنتی ویروس یا تروژان مواجه شدید لطفا آنتی ویروس ویندوز را خاموش کنید تا داناود تکمیل شود


## راه اندازی پروژه
### مشخصات سیستم من

python 3.9 , Node.js v20.11.1

از جاوا اسکریپ برای ارتباط با api freesewing و ساخت الگو مبتنی بر پارامتر های وارد شده صورت گرفته

همجنین ستاپ های مربوطه نیز درون README.txt هایی که درون فولدر های SRCCODE قرار گرفته و حتما آنهارا اجرا کنید
دستوراتی مانند npm install 

لازم به ذکر است که حتما دستورات ذکر شده را اجرا کنید تا در روند کار به ارور یا باگ برنخورید

### کتابخانه های پایتون

* کتابخانه هایی که مدل روی آنها تست شده و به خوبی کار میکند در requirements.txt قرار گرفته
* pip install -r requirements.txt




### DeepFashion2 Weights (تشخیص لندمارک ها)

* سپس لطفا فایل pose_hrnet-w48_384x288-deepfashion2_mAP_0.7017.pth را از لینک زیر دانلود کنید و در پوشه models_data واقع در SRCCODE کپی کنید
* [google-drive-download](https://drive.google.com/file/d/1hBr5tf5G0kndkQ-TKZ3CBtM7PRXxiF6j/view?usp=sharing)
* [deepfashion2-offical-github](https://github.com/svip-lab/HRNet-for-Fashion-Landmark-Estimation.PyTorch)

### Segment Anything Meta

* pip install git+https://github.com/facebookresearch/segment-anything.git


سپس این مدل های segment anything را دانلود کرده و در فولدر checkpoints واقع در SRCCODE کپی کنید


* [high-version](https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth)
* [bit-version](https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth)

## توضیحات

آموزش مدل ها و وزن های ذخیره شده آنها در پوشه AiModels صورت گرفته و فایل های جوپیتر 1 و2 و3 واقع در SRCODE نقش اپلیکیشن حاصل از آنها را دارد


در فولدر های مختلف README.txt های مختلف نوشته شده و نحوه ستاپ کردن آنها هم قرار گرفته.

## سایزبندی ها

سایز بندی بطور پیش فرض روی این ست شده و بطور کامل تست شده.

![alt text](https://i.postimg.cc/B6LrMcBP/Screenshot-2024-07-22-214905.png)

## شرایط تصاویر ورودی 

توجه : اگر تصاویر شما از قائده های زیر پیروی کند , میتوانید آنرا به مدل دهید و میتوانید تست کنید یا میتوانید از تصاویر آماده در پوشه images استفاده کنید
![alt](https://iili.io/dzeOh4R.md.png)

![alt](https://iili.io/dzeOMQa.md.png)

![alt](https://iili.io/dzeOWCJ.md.png)

## جمع بندی

لازم به ذکر است که بخش اصلی طرح همان مدل تخمین پارامتر های الگوی خیاطی بر حسب لندمارک ها است و بقیه صرفا نقش تکمیل کردن جزئیات و اپلیکیشن را دارند .

در واقع این چنین مدلی که بتواند با استفاده از لندمارک ها این پارامتر های الگوی خیاطی را تخمین بزند , برای اولین بار ساخته شده

## لینک ها

* [freesewing-api](https://github.com/freesewing/pattern-via-io)
