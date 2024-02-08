# W3-CSS
[![N|Solid](http://www.w3schools.com/images/w3schoolscom_gray.gif)](http://www.w3schools.com/w3css/default.asp)

## W3.CSS คืออะไร?
W3.CSS คือ CSS Framework ยุคใหม่ที่มาพร้อมกับฟังก์ชั่นที่มีความ responsiveness

 * เล็กกว่า และรวดเร็วกว่า CSS Framework ตัวอื่นๆ
 * เรียนรู้ ศึกษา และนำไปใช้งานได้ง่ายกว่า CSS Framework ตัวอื่นๆ
 * แค่มีความรู้ระดับพื้นฐานของ CSS ก็พร้อมที่จะไปต่อแล้ว! (หมายถึง ไม่ต้องการ JavaScript library อื่นๆ)
 * ช่วยให้งานของ Dev ง่ายขึ้นและฉับไวขึ้น
 * สนับสนุนการออกแบบแบบ Mobile First (Modern Responsive Design)
 * แสดงผลบนทุกเบราเซอร์ได้เหมือนกัน ทั้ง Chrome, Firefox, IE, Safari และอื่นๆ อีกเพียบ
 * แสดงผลบนทุกอุปกรณ์ ทุกไซส์หน้าจออย่างไม่มีที่ติ ไร้ข้อผิดพลาด
 * Type some Markdown on the left
 * See HTML in the right
 * Optimize มาเพื่อภาษาไทยเรียบร้อยแล้ว
 * จะรออะไรอีกละ! ```$ git clone``` สิครับ!

## ฟีเจอร์ในเวอร์ชั่นภาษาไทย

* ยังมีฟีเจอร์ทุกฟีเจอร์อยู่ครบ ไม่ต่างจากใน Repo เวอร์ชั่น Original
* ฟอนต์ Default ทั่วทั้งเว็บไซต์จะถูกโหลดด้วยฟอนต์ Athiti หากทำไม่ได้จะโหลดต่อด้วยฟอนต์ Sarabun แทน ทั้งภาษาไทยและภาษาอังกฤษ
* ในส่วน Heading (จาก ```<h1>``` ไปถึง ```<h6>```) จะใช้ฟอนต์ Mitr หากโหลดไม่ได้จะแทนที่ด้วย Sarabun ทั้งภาษาไทยและภาษาอังกฤษ
* ใน Class ชื่อ ```w3-code``` กับ ```w3-codespan``` ภาษาอังกฎษจะถูกโหลดด้วยฟอนต์ Consolas หรือ courier new ส่วนภาษาไทยจะถูกโหลดด้วยฟอนต์ IBM Plex Sans Thai หากโหลดไม่ได้จะใช้ Sarabun แทน
* ใน Class ชื่อ ```w3-serif``` จะโหลดฟอนต์ Serif ให้กับภาษาอังกฤษ และโหลดฟอนต์ Athiti ให้กับภาษาไทย หากโหลดไม่ได้จะใช้ Sarabun แทน
* เพิ่ม Class ชื่อ ```w3-sarabun``` สำหรับ Section  ที่่ต้องการฟอนต์ที่ดูเป็นทางการ

เนื่องจากฟอนต์ภาษาไทยดังกล่าวไม่ได้จัดอยู่ในกลุ่ม Web Safe Font จึงแนะนำให้ติดตั้งฟอนต์เหล่านี้บน Server แทน และตอนนี้ยังใช้ได้เฉพาะไฟล์ w3.css เท่านั้น

ลิสต์รายชื่อของฟอนต์ที่ต้องการ
* [Sarabun (Sarabun New)](https://www.f0nt.com/?dl_name=sipafonts/THSarabunNew.zip)
* [Athiti](https://fonts.google.com/specimen/Athiti)
* [Mitr](https://fonts.google.com/specimen/Mitr?query=Mitr&noto.lang=th_Thai)
* [IBM Plex Sans Thai](https://fonts.google.com/specimen/IBM+Plex+Sans+Thai)

## การติดตั้งฟอนต์ลงบน Front End

ในไฟล์ ```w3.css``` ให้หา Section นี้

````css
/*W3.CSS Thai Edition Font-Face Section*/
@font-face {font-family: Athiti;  src: url(Path/To/Athiti.ttf)}
@font-face {font-family: Sarabun; src: url(Sarabun.ttf)}
@font-face {font-family: Mitr;    src: url(Mitr.ttf)}
@font-face {font-family: 'IBM Plex Sans Thai';src: url('IBM Plex Sans Thai.ttf')}
````
จากนั้นให้ใส่ Path ไปที่ไฟล์ขอฟอนต์ที่ต้องการ ในส่วนของ ```src: url(ชื่อ/ของ/ฟอนต์.ttf)``` ของทุกๆ ฟอนต์ที่มีใน Section

## ติดตั้ง และ การนำไปใช้

ดาวน์โหลด Repo นี้และนำไฟล์ **w3.css** ไปใส่ในโปรเจกต์ที่ต้องการ หากจะทำผ่าน Terminal ให้ใช้คำสั่ง
```shell
$ git clone https://github.com/RouEmpire/w3.css-Thai-Edition
```

จากนั้นให้นำ Code ด้านล่างนี้ไปใส่ใน ```<head>``` ของไฟล์ HTML ที่ต้องการจะนำ Framework นี้ไปใช้

```css
<link rel="stylesheet" href="PATH/TO/w3.css">
```
เปลี่ยน Value ของ ```href``` เป็น Path ไปที่ไฟล์ w3.css ในโปรเจกต์นั้นๆ

ทดลองโดยการใส่ Code นี้ลงไปบนหน้าเว็บ
```html
<div class="w3-panel w3-grey w3-border w3-border-blue">
    <h1>ฮัลโหลๆ เทสๆ ที่คือ Mitr</h1>
    <p>อันนี้คือ Athiti</p>
    <p class="w3-sarabun">อันนี้คือ Sarabun</p>
    <p class="w3-code">อันนี้คือ IBM Plex Sans Thai</p>
</div>
```
หากคุณเห็นการแสดงผลเป็น Panel สีเทา มี Border สีน้ำเงิน และแสดงฟอนต์ถูกต้อง แปลว่า W3.CSS ได้ถูกติดตั้งเรียบร้อยแล้ว

---

หากต้องการทราบความแตกต่างระหว่าง Version ให้ตามลิงก์นี้ไปยัง w3school 

วาป : https://www.w3schools.com/w3css/w3css_versions.asp

ตามลิงก์นี้ไปเพื่อเรียนรู้เพิ่มเติมเกี่ยวกับ w3.css

วาป : http://www.w3schools.com/w3css/default.asp
