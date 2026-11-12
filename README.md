# AI Global Stock Scanner — Windows

เครื่องมือคัดกรองหุ้นต่างประเทศเพื่อการศึกษา ใช้เปิดเป็นเว็บแอปจาก Safari ผ่าน URL ของ Streamlit Community Cloud หลัง deploy หรือรันในเครื่อง Windows

## ทดลองบน Windows
1. ติดตั้ง Python 3.11+ จาก https://www.python.org/downloads/ (เลือก Add Python to PATH)
2. แตก ZIP
3. ดับเบิลคลิก `run.bat`
4. เปิด URL ที่ Streamlit แสดง (ปกติ http://localhost:8501)

## เปิดบน iPhone ผ่าน Safari
วิธีที่ง่ายคือ deploy โปรเจกต์ไปยัง Streamlit Community Cloud:
1. สร้าง GitHub account และ repository ใหม่
2. อัปโหลด `app.py` และ `requirements.txt`
3. เข้า https://share.streamlit.io/ แล้วเชื่อม GitHub
4. เลือก repository และ `app.py` แล้ว Deploy
5. เปิด URL ที่ได้บน Safari iPhone

อย่าอัปโหลด API keys, รหัสผ่าน, ข้อมูลบัญชี หรือข้อมูลส่วนตัวลง repository

## ข้อจำกัด
- ใช้ Yahoo Finance ผ่าน yfinance ซึ่งอาจล่าช้า ขาดหาย หรือเปลี่ยนแปลงได้
- คะแนนเป็น rule-based screening ไม่ใช่ AI ที่เรียนรู้เอง และไม่ใช่คำแนะนำลงทุน
- ไม่เชื่อม Dime!, ไม่ส่งคำสั่งซื้อขาย, ไม่เก็บเงินลงทุน
- ไม่ควรใช้คะแนนคัดกรองอย่างเดียวตัดสินใจซื้อขาย
