# ELUG
## Static Github Website


---

<div dir="rtl">

سلام دوستان
در این سایت که با مشارکت شما عزیزان توسعه پیدا میکنه به گسترش دانش امبدد لینوکس میپردازیم.

شما هم میتونید با تولید محتوا به اسم خودتون به ما کمک کنید.

این سایت یک static پیج که از گیت هاب برای هاست و دامین استفاده میکنه. برای توسعه سایت لازم هست یک سری موارد رو رعایت کنید.


</div>


---

## info

- page builder : Hugo
- theme : docsy


## Setup Guide

#### install Hugo

first step is you should install hugo

you can install it from source or package manager but simple way is use [this link](https://github.com/gohugoio/hugo/releases/download/v0.139.3/hugo_extended_0.139.3_linux-amd64.deb)
to install hugo extended version on ubuntu x86-64.



> hugo_extended_(version)_linux-(arch).deb

```
sudo apt install ./hugo_extended_(version)_linux-(arch).deb
```


#### install NPM

sudo apt install npm

! more dependency is needed !

#### Clone Project

```
git clone https://github.com/elugiran/elugiran.github.io.git
cd elugiran.github.io
vim content/topics/test.md
```
in test.md file:
```
## this is test
# hello world
```
for local test:
```
hugo server -D
```
for release:
```
rm -rf public/
hugo -e development
```

> :warning: حتما قبل از push دایرکتوری public را یک بار پاک کنید


#### Tips

<div dir="rtl">

 - لطفا نام فایل ها مخصوصا دایرکتوری ها را تغییر ندهید.
 - مطالبی را که قصد اضافه کردن آن را به سایت دارید در دایرکتوری content/ قرار دهید (البته با توجه به نوع مطلب چندین دسته بندی وجود دارد)
 - این سایت دستورات HTML و Script هایی را پشتیبانی میکند.
 - برای اضافه کردن یک script خاص باید تغییراتی را در فایل های اصلی قالب اضافه یا کم کنید.
- d
- d

</div>

#### site directories

| نام دایرکتوری  | توضیحات |
| ------------- |:-------------:|
|   content       | دایرکتوری اصلی برای home page     |
|   about-us      | درباره ایلاگ     |
|   meetings      | اطلاعات و فایل های دورهمی ها و event     |
|   news          | اخبار و اطلاعات مربوط به تشکیل جلسات بعدی     |
|   providers     | اسامی مهندسین ارائه دهنده مطلب در ایلاگ     |
|   topics        | موضوعات و مقالات سایت     |



#### _index.md

این فایل در صفحات تکی مانند about-us و home-page و مابقی با همین نام و مشخصات قابل تغییر میباشد بدین صورت که میتوانید هر مطبی را با توجه به


در دایرکتوری topics میتوانید فایلی با نام دلخواه و پسوند .md اضافه کنید.



## IMPORTANT !

حتما حتما قبل از push کردن به صورت لوکال local سایت را در browser تست کنید.

با این دستور :

> hugo server -D


## more info

[Hugo Quick Start](https://gohugo.io/getting-started/quick-start/)
[Docsy Get Start](https://www.docsy.dev/docs/get-started/)
