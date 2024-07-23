سلام خدمت داوران گرامی لطفا فایل SRCCODE.zip را دانلود و استخراج کنید تمامی سورس کد ها داخل موجود است. منظور Download raw file


در هنگام دانلود اگر با ارور آنتی ویروس یا تروژان مواجه شدید لطفا آنتی ویروس ویندوز را خاموش کنید تا داناود تکمیل شود.


## راه اندازی پروژه
### مشخصات سیستم من

python 3.9 , Node.js v20.11.1

از جاوا اسکریپ برای ارتباط با api freesewing و ساخت الگو مبتنی بر پارامتر های وارد شده صورت گرفته

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

سایز پیش فرض هم انتخاب شده لطفا فعلا بگذارید همین بمونه چون روی همین تست شده

![alt text](https://i.postimg.cc/B6LrMcBP/Screenshot-2024-07-22-214905.png)

## جمع بندی

لازم به ذکر است که بخش اصلی طرح همان مدل تخمین پارامتر های الگوی خیاطی بر حسب لندمارک ها است و بقیه صرفا نقش تکمیل کردن جزئیات و اپلیکیشن را دارند .

در واقع این چنین مدلی که بتواند با استفاده از لندمارک ها این پارامتر های الگوی خیاطی را تخمین بزند , برای اولین بار ساخته شده

## لینک ها

* [freesewing-api](https://github.com/freesewing/pattern-via-io)
