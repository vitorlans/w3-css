# W3-CSS
[![N|Solid](http://www.w3schools.com/images/w3schoolscom_gray.gif)](http://www.w3schools.com/w3css/default.asp)

## W3.CSS คืออะไร?
W3.CSS คือ CSS Framework ยุคใหม่ที่มาพร้อมกับสไตล์ที่มีความ Responsive

 * เล็กกว่า และรวดเร็วกว่า CSS Framework ตัวอื่นๆ
 * เรียนรู้ ศึกษา และนำไปใช้งานได้ง่ายกว่า CSS Framework ตัวอื่นๆ
 * แค่มีความรู้ระดับพื้นฐานของ CSS ก็พร้อมที่จะไปต่อแล้ว! (หมายถึง ไม่ต้องการ JavaScript library อื่นๆ)
 * ช่วยให้งานของ Dev ง่ายขึ้นและฉับไวขึ้น
 * สนับสนุนการออกแบบแบบ Mobile First (Modern Responsive Design)
 * แสดงผลบนทุกเบราเซอร์ได้เหมือนกัน ทั้ง Chrome, Firefox, IE, Safari และอื่นๆ อีกเพียบ
 * แสดงผลบนทุกอุปกรณ์ ทุกไซส์หน้าจอได้ โดยที่ไม่ต้องกังวลความ Responsive
 * Optimize มาเพื่อภาษาไทยเรียบร้อยแล้ว
 * จะรออะไรอีกละ! ```$ git clone``` สิครับ!

## ฟีเจอร์ในเวอร์ชั่นภาษาไทย

* ยังมีฟีเจอร์ทุกฟีเจอร์อยู่ครบ ไม่ต่างจากใน Repo เวอร์ชั่น Original
* ฟอนต์ Default ทั่วทั้งเว็บไซต์จะถูกโหลดด้วยฟอนต์ Noto Sans Thai หากทำไม่ได้จะโหลดต่อด้วยฟอนต์ Noto Sans แทน ทั้งภาษาไทยและภาษาอังกฤษ
* ในส่วน Heading (จาก ```<h1>``` ไปถึง ```<h6>```) จะใช้ฟอนต์ Mitr หากโหลดไม่ได้จะแทนที่ด้วย Noto Sans ทั้งภาษาไทยและภาษาอังกฤษ
* ใน Class ชื่อ ```w3-code``` , ```w3-codespan``` และ tag ชื่อ ```<code>``` , ```<pre>``` , ```<kbd>``` , ```<samp>``` ภาษาอังกฎษจะถูกโหลดด้วยฟอนต์ Consolas หรือ courier new ส่วนภาษาไทยจะถูกโหลดด้วยฟอนต์ IBM Plex Sans Thai หากโหลดไม่ได้จะใช้ Noto Sans แทน
* ใน Class ชื่อ ```w3-serif``` จะโหลดฟอนต์ Serif ให้กับภาษาอังกฤษ และโหลดฟอนต์ Noto Serif Thai ให้กับภาษาไทย หากโหลดไม่ได้จะใช้ Noto Sans แทน
* เพิ่ม Class ชื่อ ```w3-sarabun``` สำหรับ Section  ที่่ต้องการฟอนต์ที่ดูเป็นทางการ โดยจะใช้ฟอนต์ Sarabun ทั้งภาษาไทยและอังกฤษ
* เพิ่ม Class ชื่อ ```w3-sarabun-large``` สำหรับแก้ปัญหาฟอนต์ Sarabun แสดงผลเล็กเกินไป
* เมื่อฟอนต์ Noto Sans ไม่พร้อมใช้งาน จะพยายามโหลดด้วยฟอนต์ Sarabun แทนในทุกๆ Element ของเว็บ

> [!CAUTION]
> เนื่องจากฟอนต์ภาษาไทยดังกล่าวไม่ได้จัดอยู่ในกลุ่ม Web Safe Font
> จึงแนะนำให้ติดตั้งฟอนต์เหล่านี้บน Front End หรือ Host ด้วย Google Font แทน

### ลิสต์รายชื่อของฟอนต์ที่ต้องการ

เรียงลำดับตามความสำคัญจากมากไปน้อย กรณีที่เลือกใช้ทุกฟอนต์ไม่ได้
* [Noto Sans](https://fonts.google.com/noto/specimen/Noto+Sans) <sup>สำคัญมาก</sup>
* [Sarabun (Sarabun New)](https://www.f0nt.com/?dl_name=sipafonts/THSarabunNew.zip) <sup>สำคัญปานกลาง</sup>
* [Mitr](https://fonts.google.com/specimen/Mitr?query=Mitr&noto.lang=th_Thai) <sup>สำคัญปานกลาง</sup>
* [Noto Serif Thai](https://fonts.google.com/noto/specimen/Noto+Serif+Thai) <sup>สำคัญน้อย</sup>
* [IBM Plex Sans Thai](https://fonts.google.com/specimen/IBM+Plex+Sans+Thai) <sup>สำคัญน้อย</sup>


## การติดตั้งฟอนต์ลงบน Front End

ในไฟล์ ```w3.css``` , ```w3pro.css``` , ```w3mobile.css``` ให้หา Section นี้

````css
/*W3.CSS Thai Edition Font-Face Section*/
@font-face {font-family: 'TH Sarabun New'     ;src: url('TH Sarabun New.ttf')}
@font-face {font-family: 'Mitr '              ;src: url('Mitr.ttf')}
@font-face {font-family: 'Noto Serif Thai'    ;src: url('Noto Serif Thai.ttf');}
@font-face {font-family: 'Noto Sans'          ;src: url('Noto Sans.ttf')}
@font-face {font-family: 'IBM Plex Sans Thai' ;src: url('IBM Plex Sans Thai.ttf')}
````
จากนั้นให้ใส่ Path ไปที่ไฟล์ของฟอนต์ที่ต้องการ ในส่วนของ ```src: url(ชื่อ/ของ/ฟอนต์.ttf)``` ของทุกๆ ฟอนต์ที่มีใน Section

## ติดตั้ง และ การนำไปใช้

ดาวน์โหลด Repo นี้และนำไฟล์ **w3.css** หรือไฟล์อื่นๆ ที่ต้องการนำไปใช้ ไปใส่ในโปรเจกต์ที่ต้องการ หากจะทำผ่าน Terminal ให้ ```cd``` ไปที่โฟลเดอร์ของ Project ของท่าน และใช้คำสั่งนี้ (ให้เปลีี่ยน ```-b master``` เป็น ```-b beta``` หากต้องการติดตั้งเวอร์ชั่นทดสอบ)

```shell
git clone -b master https://github.com/RouEmpire/w3.css-Thai-Edition
```



จากนั้นให้นำ Code ด้านล่างนี้ไปใส่ใน ```<head>``` ของไฟล์ HTML ที่ต้องการจะนำ Framework นี้ไปใช้

```css
<link rel="stylesheet" href="w3.css-Thai-Edition/w3.css">
```
เปลี่ยน Value ของ ```href``` เป็น Path ไปที่ไฟล์ w3.css ในโปรเจกต์นั้นๆ

ทดลองโดยการใส่ Code นี้ลงไปบนหน้าเว็บ
```html
<div class="w3-container">
    <div class="w3-panel w3-light-blue w3-border w3-border-blue w3-leftbar">
        <h1>ฮัลโหลๆ เทสๆ ที่คือ Mitr</h1>
        <p>อันนี้คือ Athiti</p>
        <code class="w3-sarabun">อันนี้คือ Sarabun ที่อยู่ใน <strong>w3-sarabun</strong> </code>
        <p class="w3-code">อันนี้คือ IBM Plex Sans Thai ที่อยู่ใน <strong>w3-code</strong> </p>
        <code class="w3-code w3-black w3-leftbar w3-border-purple">แต่อันนี้ีเจ๋งกว่า</code>
        <code class="w3-serif w3-border-purple">อันนี้คือ Serif ที่อยู่ใน <strong>w3-serif</strong></code>
        <h6> ส่วนนี่คือ h6</h6>
        <p> <span class="w3-sarabun"> [อันนี้ w3-sarabun] </span> <span class="w3-sarabun-large"> [อันนี้ w3-sarabun-large] </span> [เทียบกับ Athiti] <span class="w3-code">อันนี้ w3-code</span></p>
    </div>
</div>
```
หากคุณเห็นการแสดงผลเป็น Panel สีฟ้า มี Border สีน้ำเงิน และแถบของ ```w3-code``` 2 แถบ (สีดำกับสีขาว) แปลว่า W3.CSS ได้ถูกติดตั้งเรียบร้อยแล้ว แต่ถ้าหากยังแสดงฟอนต์ผิดพลาด ให้พยายามตรวจสอบชื่อของไฟล์ฟอนต์ที่ใส่ และ Path ที่พามายังฟอนต์ 

## Todo

* ทดสอบ และทำให้ใช้งานร่วมกับ Google Font ได้ง่ายขึ้น
* แก้ปัญหา Size ของฟอนต์ที่แสดงผลไม่เท่ากันทั่วทั้งเว็บไซต์ในบางเบราเซอร์
---

หากต้องการทราบความแตกต่างระหว่าง Version ให้ตามลิงก์นี้ไปยัง w3school 

วาป : https://www.w3schools.com/w3css/w3css_versions.asp

ตามลิงก์นี้ไปเพื่อเรียนรู้เพิ่มเติมเกี่ยวกับ w3.css

วาป : http://www.w3schools.com/w3css/default.asp
