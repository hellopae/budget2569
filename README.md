# บัญชีรายรับ-รายจ่าย 2569

โปรแกรมบันทึกรายรับ-รายจ่าย ปี พ.ศ. 2569 (ธุรกิจ — แยกตามบริษัท/ลูกค้า)

## Features
- ปฏิทินรายเดือน 12 เดือน — แต่ละรายการแสดง **ชื่อบริษัท + ยอด** สีเขียว(รับ)/แดง(จ่าย)
- รายชื่อบริษัท/ลูกค้าให้เลือก (quick-pick) + จัดการรายชื่อในหน้าตั้งค่า
- สรุปรายเดือน: รายรับ/รายจ่าย, **สรุปตามบริษัท**, เงินยกมา, วงเงิน OD, กำไรสุทธิ
- พิมพ์/บันทึก PDF (ปฏิทิน / สรุป / ทั้งหมด)
- **Cloud sync ผ่าน Firebase** — login ด้วยอีเมล แล้วข้อมูล sync ทุกเครื่อง (คอม/มือถือ)
- ทำงาน offline ได้ (เก็บใน LocalStorage) และ sync ขึ้น cloud อัตโนมัติเมื่อ login

## ใช้งาน
เปิดผ่าน [GitHub Pages](https://hellopae.github.io/budget2569/)

## ตั้งค่า Cloud (Firebase)
- ค่า config อยู่ในตัวแปร `firebaseConfig` ใน `index.html`
- ต้องเปิด Authentication (Email/Password) + Firestore + วาง Security Rules ในโปรเจกต์ Firebase
- โดเมนที่ deploy (เช่น `hellopae.github.io`) ต้องเพิ่มใน Firebase → Authentication → Settings → Authorized domains
