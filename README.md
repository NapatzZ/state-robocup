# RoboCup@Home Task State Flowchart

Repository รวบรวม flowchart task ต่างๆ ใน RoboCup@Home โดยใช้ Mermaid Chart เพื่อแสดงผัง State Flow ของแต่ละ Task

---

## 📋 Task Documentation

### Restaurant 

**Task Description**: Robot ทำหน้าที่เป็นพนักงานเสิร์ฟในร้านอาหาร โดยต้องตรวจจับลูกค้าที่เรียก รับออเดอร์ และนำอาหารไปเสิร์ฟ

**Main Goal**: 
- ตรวจจับลูกค้าที่เรียกหรือโบกมือ
- ไปยังโต๊ะลูกค้าโดยไม่ต้องมีการนำทาง
- รับและเสิร์ฟออเดอร์ทั้งหมด

**Optional Goal**: ใช้ถาดในการขนส่งออเดอร์

**Key Features**:
- ทำงานในร้านอาหารจริงที่ไม่เคยรู้จักมาก่อน
- มีลูกค้าจริงและลูกค้าทดสอบ (Professional Customers)
- ใช้เวลาสูงสุด 15 นาที
- คะแนนเต็ม 2000 คะแนน

**🔗 Link to Flowchart**: [Restaurant.md](Restaurant.md)

---

### Storing Groceries [StoringGroceries.md]

**Task Description**: Robot ต้องจัดเก็บของชำลงในตู้โดยการจัดกลุ่มตามหมวดหมู่หรือความคล้ายคลึงกัน

**Main Goal**: 
- ย้ายของจากโต๊ะไปยังตู้ โดยจัดกลุ่มตามหมวดหมู่
- เติมซีเรียลลงในภาชนะที่กำหนด

**Optional Goals**:
1. เปิดประตูตู้
2. ย้ายของขนาดเล็ก
3. ย้ายของหนัก
4. หยิบของจากถุงช้อปปิ้ง

**Key Features**:
- มีของบนโต๊ะ 5-10 ชิ้น และในถุงช้อปปิ้ง 5-10 ชิ้น
- ต้องจัดกลุ่มของตามหมวดหมู่ที่มีอยู่ในตู้
- ต้องเทซีเรียลลงในภาชนะที่เปิดไว้
- ใช้เวลาสูงสุด 7 นาที
- คะแนนเต็ม 1890 คะแนน

**🔗 Link to Flowchart**: [StoringGroceries.md](StoringGroceries.md)

---
