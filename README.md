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

**Scoring System**:

| Action | Score |
|--------|-------|
| **Regular Rewards** | |
| Detect calling or waving customer | 2×100 |
| Reach a customer's table without prior guidance/training | 2×100 |
| Understand and confirm the order received to the customer | 2×200 |
| Communicate the order to the barman | 2×100 |
| Return to the customer table with the order | 2×100 |
| Serve the order to the customer | 2×200 |
| **Bonus Rewards** | |
| Use an unattached tray to transport | 2×200 |
| **Regular Penalties** | |
| Being guided to a table | 2×-200 |
| Not making eye-contact when taking an order | 2×-80 |
| Not reaching the bar (barman has to move from behind the bar) | 2×-80 |
| **Deus ex Machina Penalties** | |
| Asking the Barman to handover object to the robot | 4×-50 |
| Guest needing to take the object from a tray or robot's hand | 4×-50 |
| Being told/pointed where is a table/Kitchen-bar | 2×-100 |

**🔗 Link to Flowchart**: [Restaurant.md](Restaurant.md)

---

### Storing Groceries

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

**Scoring System**:

| Action | Score |
|--------|-------|
| **Main Goal** | |
| Navigating to the table | 15 |
| Perceiving object and categorizing it correctly | 5×15 |
| Picking up an object for transportation to the cabinet | 5×50 |
| Perceiving objects in shelf and saying on which layer the currently handled object should be placed | 5×15 |
| Placing an object in the cabinet | 5×15 |
| Placing an object next to similar objects on the cabinet | 5×50 |
| Opening the first cabinet door | 200 |
| Opening the second cabinet door | 100 |
| Pouring cereal into the container | 300 |
| **Bonus Rewards** | |
| Picking up an object from the shopping bag | 5×50 |
| Picking up a tiny object | 30 |
| Placing a tiny object | 70 |
| Picking up a heavy object | 70 |
| Placing a heavy object | 30 |
| Autonomously Picking any Object | 50 |
| Autonomously Placing any Object | 50 |
| **Deus Ex Machina Penalties** | |
| Perceiving object and categorizing it wrongly | 10×-15 |
| A human handing an object over to the robot | 5×-50 |
| A human placing an object in the cabinet | 5×-15 |
| A human placing an object in the cabinet next to similar objects | 5×-50 |
| A human pointing at a target location | 5×-25 |
| A human opening the first cabinet door | -200 |
| A human opening the second cabinet door | -100 |
| Spilling cereal while pouring | -100 |
| Leaving cereal in the box | -300 |
| A human pouring cereal in the bowl | -300 |

**🔗 Link to Flowchart**: [StoringGroceries.md](StoringGroceries.md)

---
