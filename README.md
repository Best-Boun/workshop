# E-Commerce Platform for Computer Hardware and Gaming Gears

**สมาชิก**
- สุรวุฒิ บุญยู้
- เชษฐกิตติ์ สืบสุขสันติ
- รัชภูมิ ธรรมประชา
- ภูริภัทร ทองมวน

## หลักการและเหตุผล

- ปัจจุบันความต้องการอุปกรณ์คอมพิวเตอร์และเกมมิ่งเกียร์เติบโตขึ้นอย่างมาก แต่ผู้ซื้อมักเจอปัญหาร้านค้าออนไลน์ที่ใช้งานยากและจัดหมวดหมู่ซับซ้อน คณะผู้จัดทำจึงพัฒนาระบบ    E-commerce นี้ขึ้น เพื่อสร้างแพลตฟอร์มจำลองที่ซื้อขายง่าย ค้นหาสินค้าได้สะดวก และแยกหมวดหมู่อุปกรณ์ชัดเจน เพื่อตอบโจทย์พฤติกรรมของผู้บริโภคยุคดิจิทัลได้อย่างมีประสิทธิภาพ

## วัตถุประสงค์ของโครงงาน

- เพื่อพัฒนาเว็บแอปพลิเคชัน E-commerce สำหรับซื้อขายอุปกรณ์คอมพิวเตอร์ที่ค้นหาง่ายและแยกหมวดหมู่ชัดเจน
- เพื่อพัฒนาระบบตะกร้าสินค้าที่สามารถคำนวณเงิน ปรับเพิ่ม/ลดจำนวน และสรุปยอดสั่งซื้อได้อย่างถูกต้อง

## ขอบเขตของระบบ

**ผู้ใช้งาน**
- ลูกค้า
- ผู้ดูแลระบบ
- ผู้จัดการ

**ความสามารถของระบบ**
1. สมัครสมาชิก / เข้าสู่ระบบ
2. ดูและค้นหาสินค้า
3. เพิ่มสินค้าใส่รถเข็น
4. สั่งซื้อสินค้า
5. ผู้ดูแลระบบจัดการสินค้าและคำสั่งซื้อ

## แนวทางการพัฒนาตาม SDLC

1. ประชุมเลือกหัวข้อ กำหนดขอบเขตระบบ และแบ่งงานในกลุ่ม
2. รวบรวมข้อมูลสินค้าและวิเคราะห์ความต้องการหน้าจอของระบบ
3. ออกแบบ UI/UX ด้วย Figma และออกแบบโครงสร้างฐานข้อมูล (Database Schema)
4. พัฒนา Frontend ด้วย React และพัฒนา Backend ด้วย Node.js เชื่อมต่อกับ MySQL
5. ทดสอบระบบแบบ
6. นำระบบขึ้นระบบจำลองหรือคลาวด์เซิร์ฟเวอร์
7. ตรวจสอบและแก้ไขข้อผิดพลาด

## เครื่องมือแล้วเทคโนโลยีที่ใช้

**Frontend**
- HTML/CSS/Javascript
- React
- Boostrap

**Backend**
- Node.js

**Database**
- Local Storage

**Design Tool**
- Figma

**Version Control**
- Github

## แนวทางในการทดสอบระบบ

**ประเภทการทดสอบ**
- User Acceptance Testing (UAT)

**เครื่องมือที่ใช้**
- Manual Testing

## ผลลัพท์ที่คาดว่าจะได้รับ

1. ระบบสามารถแสดงรายการสินค้าและราคาอุปกรณ์คอมพิวเตอร์แยกตามหมวดหมู่ได้อย่างถูกต้อง
2. ระบบสามารถบันทึก ปรับปรุง และคำนวณราคาสินค้าในตะกร้าของลูกค้าได้แบบเรียลไทม์
3. ระบบสามารถจำลองการออกใบสรุปยอดเงินและประวัติการสั่งซื้อหลังสิ้นสุดขั้นตอนชำระเงิน
4. ข้อมูลการเลือกซื้อสินค้าถูกจัดเก็บใน Local Storage ได้อย่างถูกต้องและปลอดภัยฝั่งผู้ใช้

## แผนการดำเนินงาน

1. เก็บรวบรวมความต้องการของระบบ, ออกแบบ UI/UX ด้วย Figma และออกแบบโครงสร้างฐานข้อมูล (Database Schema)น Local Storage ได้อย่างถูกต้องและปลอดภัยฝั่งผู้ใช้
2. เขียนโค้ดส่วนหน้าบ้านด้วย React เพื่อสร้างหน้าจอแสดงสินค้า หมวดหมู่ ตะกร้าสินค้า และหน้าจำลองสั่งซื้อ
3. พัฒนาส่วนหลังบ้านด้วย Node.js และสร้างฐานข้อมูล MySQL เพื่อใช้จัดการและเชื่อมต่อข้อมูลสินค้าและคำสั่งซื้อ
4. ทำการทดสอบระบบแบบ Manual Testing และทำ UAT ตรวจสอบความถูกต้อง พร้อมจัดทำสรุปเพื่อนำเสนอผลงาน

## Screenshot SourceTree 

![Logo](images/Screenshot.png)


## System Architecture

```mermaid
flowchart TB

%% =========================
%% CUSTOMER
%% =========================
subgraph CUSTOMER["👤 CUSTOMER"]
direction LR
A[Register / Login]
B[Home]
C[Browse Products]
D[Product Details]
E[Shopping Cart]
F[Checkout]
G[Payment]
H[Order Complete]
I[Order History]

A --> B --> C --> D --> E --> F --> G --> H --> I
end

%% =========================
%% ADMIN
%% =========================
subgraph ADMIN["🛠️ ADMINISTRATOR"]
direction TB

AA[Admin Login]
AB[Dashboard]

AA --> AB

AB --> AC[Manage Products]
AB --> AD[Manage Categories]
AB --> AE[Manage Orders]
AB --> AF[Manage Users]

end

%% =========================
%% BACKEND
%% =========================
subgraph BACKEND["⚙️ BACKEND (Node.js)"]
direction LR

BA[Authentication]
BB[Product Service]
BC[Cart Service]
BD[Order Service]
BE[User Service]
BF[Admin Service]
BG[REST API]

end

%% =========================
%% DATABASE
%% =========================
subgraph DATABASE["🗄️ DATABASE / STORAGE"]
direction LR

DA[(Users)]
DB[(Categories)]
DC[(Products)]
DD[(Cart)]
DE[(Orders)]
DF[(Order Items)]
DG[(Payments)]

end

%% =========================
%% CONNECTIONS
%% =========================

CUSTOMER --> BACKEND
ADMIN --> BACKEND

BA --> DA
BB --> DB
BB --> DC
BC --> DD
BD --> DE
BD --> DF
BD --> DG
BE --> DA
BF --> DA

## 1) แผนภาพกรณีการใช้งาน (Use Case Diagram)

```mermaid
flowchart LR
  CUST[ลูกค้า]
  ADM[ผู้ดูแลระบบ]
  SADM[ผู้ดูแลสูงสุด]

  subgraph SYS[ระบบร้านค้าออนไลน์ TechPulse]
    UC1((สมัครสมาชิก))
    UC2((เข้าสู่ระบบด้วยอีเมลหรือกูเกิล))
    UC3((ดูรายการสินค้าและค้นหา))
    UC4((กรองสินค้าตามหมวดหมู่และยี่ห้อ))
    UC5((ดูรายละเอียดสินค้า))
    UC6((เพิ่มสินค้าลงตะกร้า))
    UC7((ยืนยันคำสั่งซื้อและกรอกที่อยู่จัดส่ง))
    UC8((ชำระเงินและตรวจสอบสถานะการชำระ))
    UC9((ติดตามคำสั่งซื้อและดูประวัติคำสั่งซื้อ))
    UC10((จัดการข้อมูลบัญชีส่วนตัว))

    UC11((จัดการสินค้า เพิ่ม แก้ไข ลบ))
    UC12((จัดการหมวดหมู่สินค้า))
    UC13((จัดการคำสั่งซื้อและอัปเดตสถานะจัดส่ง))
    UC14((จัดการข้อมูลลูกค้า))
    UC15((ดูรายงานสรุปและสถิติแดชบอร์ด))
    UC16((ตรวจสอบประวัติการใช้งานและความปลอดภัย))
    UC17((จัดการสิทธิ์การเข้าถึงของผู้ดูแลระบบ))
  end

  CUST --> UC1
  CUST --> UC2
  CUST --> UC3
  CUST --> UC4
  CUST --> UC5
  CUST --> UC6
  CUST --> UC7
  CUST --> UC8
  CUST --> UC9
  CUST --> UC10

  ADM --> UC11
  ADM --> UC12
  ADM --> UC13
  ADM --> UC14
  ADM --> UC15
  ADM --> UC16

  SADM --> UC16
  SADM --> UC17
```

หน้าที่ของแผนภาพ:
- แสดงขอบเขตของระบบ TechPulse ให้เห็นชัดว่าใครทำอะไรได้บ้าง
- ใช้ยืนยันขอบเขตงานกับสมาชิกในทีมและผู้สอน

ความสำคัญต่อการพัฒนาระบบ:
- ลดความเสี่ยงการตกหล่นฟังก์ชันสำคัญ เช่น ตรวจสิทธิ์และงานหลังบ้าน
- ใช้เป็นฐานในการกำหนดเส้นทางหน้าเว็บและสิทธิ์การเรียก API ตามบทบาท

## 2) แผนภาพคลาส (Class Diagram)

หมายเหตุ: แผนภาพนี้อ้างอิงชื่อโครงสร้างข้อมูลจริงในฐานข้อมูลของโครงการ

```mermaid
classDiagram
  class User {
    +int id
    +string first_name
    +string last_name
    +string email
    +string password
    +string role
    +json permissions
    +datetime created_at
    +datetime updated_at
  }

  class Category {
    +int id
    +string name
    +string image
    +datetime created_at
    +datetime updated_at
  }

  class Product {
    +int id
    +int category_id
    +string sku
    +string name
    +string brand
    +string description
    +decimal price
    +int stock
    +string status
    +bool featured
  }

  class Order {
    +int id
    +int user_id
    +decimal total_price
    +string status
    +string shipping_name
    +string shipping_phone
    +string shipping_address
    +string shipping_city
    +string shipping_postal_code
    +string shipping_country
    +datetime created_at
    +datetime updated_at
  }

  class OrderItem {
    +int id
    +int order_id
    +int product_id
    +int quantity
    +decimal price
    +decimal subtotal
    +datetime created_at
  }

  class Payment {
    +int id
    +int order_id
    +string payment_method
    +string payment_status
    +string transaction_id
    +decimal amount
    +datetime paid_at
    +datetime created_at
  }

  User "1" --> "0..*" Order : สร้างคำสั่งซื้อ
  Category "1" --> "0..*" Product : จัดกลุ่มสินค้า
  Order "1" --> "1..*" OrderItem : มีรายการสินค้า
  Product "1" --> "0..*" OrderItem : ถูกอ้างอิงในรายการสั่งซื้อ
  Order "1" --> "0..*" Payment : เชื่อมข้อมูลการชำระเงิน
```

หน้าที่ของแผนภาพ:
- แสดงโครงสร้างข้อมูลหลักและความสัมพันธ์ระหว่างเอนทิตีในระบบ
- ใช้อ้างอิงร่วมกันระหว่างการออกแบบฐานข้อมูลและการพัฒนาโมเดล

ความสำคัญต่อการพัฒนาระบบ:
- ลดความกำกวมของข้อมูล เช่น ความสัมพันธ์ Order กับ OrderItem และ Payment
- ป้องกันการออกแบบซ้ำซ้อน ทำให้พัฒนา Controller และ Service ได้สอดคล้องกัน

## 3) แผนภาพลำดับงาน (Sequence Diagram)

กรณีศึกษา: ลำดับการทำงานของการสั่งซื้อและการชำระเงินในระบบจริง

```mermaid
sequenceDiagram
  autonumber
  actor C as ลูกค้า
  participant FE as ส่วนหน้าเว็บ React
  participant BE as ส่วนหลังเว็บ Express
  participant OM as ตัวจัดการคำสั่งซื้อ
  participant PM as ตัวจัดการชำระเงิน
  participant DB as ฐานข้อมูล MySQL

  C->>FE: กดยืนยันสั่งซื้อ
  FE->>BE: ส่งคำขอสร้างคำสั่งซื้อ พร้อมโทเคนและข้อมูลจัดส่ง
  BE->>OM: เริ่มสร้างคำสั่งซื้อ
  OM->>DB: เริ่มธุรกรรม
  OM->>DB: ตรวจสต็อกและล็อกข้อมูลสินค้า
  OM->>DB: บันทึกคำสั่งซื้อและรายการสินค้า
  OM->>DB: ตัดจำนวนสต็อกสินค้า
  OM->>DB: ยืนยันธุรกรรม
  OM-->>BE: ส่งรหัสคำสั่งซื้อกลับ
  BE-->>FE: ตอบกลับว่าสร้างคำสั่งซื้อสำเร็จ

  C->>FE: เลือกวิธีชำระเงินและยืนยัน
  FE->>BE: ส่งคำขอประมวลผลการชำระเงิน
  BE->>PM: ประมวลผลการชำระเงิน
  PM->>DB: บันทึกข้อมูลการชำระเงิน
  PM-->>BE: ส่งสถานะการชำระเงิน
  BE-->>FE: ตอบกลับผลลัพธ์สำเร็จหรือรอดำเนินการหรือไม่สำเร็จ
  FE-->>C: แสดงผลการชำระเงินและสถานะคำสั่งซื้อ
```

หน้าที่ของแผนภาพ:
- แสดงลำดับการเรียกใช้งานจริงจากผู้ใช้ไปจนถึงฐานข้อมูล
- ช่วยให้ทีมเห็นจุดที่ต้องมีการตรวจสอบสิทธิ์ ตรวจสต็อก และควบคุมธุรกรรม

ความสำคัญต่อการพัฒนาระบบ:
- ทำให้มองเห็นจุดเสี่ยงด้านความถูกต้องของข้อมูล เช่น การตัดสต็อกซ้ำ
- ใช้ระบุจุดคอขวดที่ทำให้ระบบช้าในช่วงผู้ใช้หนาแน่น

