# 🧳 นัดวันไปเที่ยว

เว็บให้เพื่อนใส่ชื่อ เลือกวันที่ว่างบนปฏิทิน แล้วดูว่าวันไหนว่างตรงกันมากที่สุด (อัปเดตอัตโนมัติ) แต่ละคนกลับมาแก้วันของตัวเองได้โดยพิมพ์ชื่อเดิมหรือกดชื่อในรายชื่อ

## ตั้งค่าให้ใช้งานได้

1. สร้างโปรเจกต์ที่ https://console.firebase.google.com (แผน Spark ฟรี)
2. Build → Firestore Database → Create database (location `asia-southeast1`, production mode)
3. แท็บ **Rules** → วางเนื้อหาจากไฟล์ `firestore.rules` → **Publish**
4. Project settings → Your apps → เพิ่มแอป Web (`</>`) → คัดลอก `firebaseConfig`
5. แก้ไฟล์ `index.html` วาง `firebaseConfig` แทนค่าว่างใกล้ท้ายไฟล์ แล้ว commit
6. Settings → Pages → Source: **Deploy from a branch** → Branch `main` / `(root)` → Save

เว็บจะอยู่ที่ `https://thanadonsn.github.io/vacationplanning/`
