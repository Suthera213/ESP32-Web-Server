# การทดลอง Webserver อย่างง่ายด้วย ESP32

##  ขั้นตอนการทดลอง 
### 1. สร้าง Project ใหม่ ชื่อ ESP32-Web-Server


![Alt text](./Pictures/1.Create-new-project.png)

1.1 ใช้ template simple server

![Alt text](./Pictures/2.Select-project-template.png)


###  2. Build โปรเจค 1 ครั้ง 
เพื่อให้ระบบสร้างไฟล์ sdkconfig เราจะเข้าไปแก้ WiFI ssid และ password
 
![Alt text](./Pictures/3.Edit-SSID-snd-Password.png)

###  3. รันโปรแกรม แก้ไขที่ผิด (ถ้ามี)

![Alt text](./Pictures/4.Found-Error.png)

พบ error เนื่องจากค่าเริ่มต้นของโปรแกรมกำหนดให้ความยาวของ HTTP request header มีต่าสูงสุด 152 ตัวอักษร เราต้องแก้ให้เป็น 1024 

###  4. แก้ไข Max HTTP Request Header Lenght เป็น 1024

![Alt text](./Pictures/5.Change-Req-Header-Len.png)

###  5. รันโปรแกรม แก้ไขที่ผิด (ถ้ามี)


ตัวอย่างผลการทำงาน (เมื่อดูจาก browser)
![Alt text](./Pictures/6.Sample-Result.png)


###  6. บันทึกผลการทดลอง ทั้งที่หน้าจอ monitor ของ ESP32 และหน้า Web browser
![277099269-f518569b-5d61-44b4-b2e3-ed7ab86f1453](https://github.com/Suthera213/ESP32-Web-Server/assets/115066359/c3d28760-b1a6-4caa-aa7a-fcc495652295)

![image](https://github.com/Suthera213/ESP32-Web-Server/assets/115066359/579a795b-5d6c-4a7c-ae0f-b74341d26ef7)

###  7. ส่งงาน
pull request พร้อมแนบ link ไปยัง repository ของโปรเจคด้วยนะ
https://github.com/Suthera213/web-sever


