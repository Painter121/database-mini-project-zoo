# Database Mini Project — Zoo Management System

โครงงานระบบบริหารจัดการสวนสัตว์ออนไลน์ พัฒนาขึ้นในรายวิชา Database (ปี 2 เทอม 2) โดยออกแบบสถาปัตยกรรมฐานข้อมูลเชิงสัมพันธ์ (Relational Database) และพัฒนาเว็บแอปพลิเคชันสำหรับจัดการข้อมูลด้วย Node.js, Express และ MySQL

## ขอบเขตและฟังก์ชันระบบ

- **ระบบจัดการข้อมูลสัตว์และที่อยู่อาศัย:** จัดการข้อมูลสัตว์, สายพันธุ์, การจำแนกประเภท (Category), และโซนที่อยู่อาศัย (Habitat Zones)
- **ระบบบันทึกสุขภาพและการดูแล (Animal Care):** ติดตามประวัติการรักษาพยาบาล, ตารางให้อาหาร, และการดูแลสุขภาพสัตว์
- **ระบบจัดการบุคลากร (Employee):** บันทึกข้อมูลพนักงาน, ตำแหน่งหน้าที่, และการมอบหมายงานดูแลในแต่ละโซน
- **ระบบสมาชิกและผู้เข้าชม (Visitor & Favorites):** ระบบสมัครสมาชิก, เข้าสู่ระบบ, และการบันทึกสัตว์ที่ชื่นชอบ
- **แดชบอร์ดสรุปผล:** แสดงข้อมูลสถิติภาพรวมของสวนสัตว์
- **สถาปัตยกรรมฐานข้อมูล:** ออกแบบตามหลัก Normalization พร้อมรองรับการ Query ข้อมูลที่ซับซ้อน (Multi-table JOIN, SubQuery, Stored Procedure และ Database Triggers)

## เทคโนโลยีที่ใช้

- **Backend:** Node.js, Express.js
- **Database:** MySQL
- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **Security:** Password Hashing (bcrypt), JWT, Environment Variables (.env)

## วิธีการติดตั้งและรันโปรเจกต์

1. **เตรียมฐานข้อมูล:**
   - นำเข้าโครงสร้างฐานข้อมูลจากไฟล์ `database/schema.sql` ลงใน MySQL (เช่น ผ่าน phpMyAdmin หรือ MySQL Workbench)
2. **ตั้งค่า Environment:**
   - คัดลอกไฟล์ `.env.example` เป็น `.env` ในโฟลเดอร์ `NodeJsSystem`
   - กำหนดค่าการเชื่อมต่อฐานข้อมูล (DB_HOST, DB_USER, DB_PASSWORD, DB_NAME)
3. **ติดตั้ง Dependencies และรัน Server:**
   ```bash
   cd NodeJsSystem
   npm install
   npm start
   ```
4. เปิดเบราว์เซอร์แล้วเข้าใช้งานที่ `http://localhost:3000`
