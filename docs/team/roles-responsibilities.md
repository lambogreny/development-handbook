# 🧩 บทบาทและหน้าที่ในองค์กร

เอกสารนี้อธิบายบทบาท หน้าที่รับผิดชอบ และความเกี่ยวข้องในกระบวนการทำงานของแต่ละตำแหน่งในองค์กร

---

## 📊 โครงสร้างองค์กรและสายการบังคับบัญชา

```
ผู้จัดการทั่วไป (General Manager)
        │
        ├── หัวหน้า Dev (Tech Lead)
        │     ├── Backend Developer (API)
        │     └── Frontend Developer
        │
        ├── UX/UI Designer
        │
        ├── Product Manager (PM)
        │
        └── Quality Assurance (QA)
```

---

## 👨‍💼 ผู้จัดการทั่วไป (General Manager)

### บทบาทและความรับผิดชอบ:

- กำหนดทิศทางและกลยุทธ์ของผลิตภัณฑ์และองค์กรโดยรวม
- อนุมัติงบประมาณและทรัพยากรสำหรับโปรเจกต์
- ตัดสินใจเชิงธุรกิจที่ส่งผลต่อไทม์ไลน์และคุณภาพของผลิตภัณฑ์
- ประสานงานกับลูกค้าและผู้มีส่วนได้ส่วนเสียระดับสูง
- ดูแลประสิทธิภาพของทีมโดยรวมและแก้ไขปัญหาขัดแย้ง

### ความเกี่ยวข้องใน Development Flow:

- **เริ่มต้นโปรเจกต์**: อนุมัติโปรเจกต์และกำหนดเป้าหมายธุรกิจ
- **Milestone Approval**: ทบทวนและอนุมัติ milestone สำคัญ
- **Risk Management**: รับทราบและจัดการความเสี่ยงระดับสูง
- **เมื่อเกิดปัญหาวิกฤต**: เข้ามาตัดสินใจเมื่อมีผลกระทบต่อธุรกิจ (เช่น เลื่อน deadline, เพิ่มงบประมาณ)
- **Release Approval**: อนุมัติการ release เวอร์ชันสำคัญไปยัง Production

---

## 👨‍💻 หัวหน้า Dev (Tech Lead)

### บทบาทและความรับผิดชอบ:

- ออกแบบสถาปัตยกรรมระบบและแนวทางเทคนิค
- นำทีมพัฒนาและแก้ไขปัญหาทางเทคนิคที่ซับซ้อน
- กำหนดมาตรฐานการเขียนโค้ดและแนวทางการพัฒนา
- ทบทวนและอนุมัติ Pull Request
- วางแผนและจัดสรรงานให้ Developer
- บริหารจัดการ Technical Debt
- ดูแล DevOps และกระบวนการ CI/CD

### ความเกี่ยวข้องใน Development Flow:

- **Sprint Planning**: กำหนดงานด้านเทคนิคและประเมินความยากง่าย
- **Architecture Design**: ออกแบบและเอกสารเชิงเทคนิค
- **Code Review**: ตรวจสอบและอนุมัติ PR จาก Dev ทุกคน
- **Technical Decision**: ตัดสินใจเรื่องเทคโนโลยีและแนวทางการพัฒนา
- **Merge & Deploy**: ดูแลการ merge code เข้า develop และ main
- **Hotfix**: รับผิดชอบการแก้ไขปัญหาฉุกเฉินใน production
- **Technical Support**: ให้คำปรึกษาทางเทคนิคแก่ทีม Dev

---

## 🧑‍💻 Backend Developer (API)

### บทบาทและความรับผิดชอบ:

- พัฒนา API และ Backend Services ตาม requirement
- ออกแบบและพัฒนาฐานข้อมูล
- เขียนเอกสาร API Documentation
- พัฒนา Unit Tests สำหรับ Backend Code
- ดูแลประสิทธิภาพและความปลอดภัยของระบบ
- มีส่วนร่วมใน Code Review

### ความเกี่ยวข้องใน Development Flow:

- **Feature Implementation**: พัฒนา feature บน branch แยก `feature/*`
- **API Design**: ออกแบบ API ร่วมกับ Frontend Developer และ Tech Lead
- **Self Testing**: ทดสอบ API ด้วยตนเองก่อนส่ง PR
- **Code Review**: ส่ง PR และปรับแก้ตาม feedback
- **Documentation**: เขียน API documentation และตัวอย่างการใช้งาน
- **Bug Fixing**: แก้ไขบัคที่พบโดย QA หรือ Frontend Dev
- **Database Management**: ออกแบบและปรับปรุงโครงสร้างฐานข้อมูล

---

## 👩‍💻 Frontend Developer

### บทบาทและความรับผิดชอบ:

- พัฒนา User Interface ตามแบบของ UX/UI Designer
- เชื่อมต่อกับ API ที่ Backend Developer พัฒนา
- พัฒนา responsive design และ cross-browser compatibility
- ทำ client-side validation และ error handling
- พัฒนา unit tests สำหรับ Frontend code
- ดูแลประสิทธิภาพและ user experience

### ความเกี่ยวข้องใน Development Flow:

- **Feature Implementation**: พัฒนา feature บน branch แยก `feature/*`
- **UI Development**: พัฒนา UI ตามแบบจาก UX/UI Designer
- **API Integration**: เชื่อมต่อกับ API จาก Backend Developer
- **Self Testing**: ทดสอบ UI และฟังก์ชันบนหลาย browser/device ก่อนส่ง PR
- **Code Review**: ส่ง PR และปรับแก้ตาม feedback
- **Bug Fixing**: แก้ไขบัคที่พบโดย QA หรือ UX/UI Designer
- **UI/UX Feedback**: ให้ feedback เชิงเทคนิคต่อ UX/UI design

---

## 🎨 UX/UI Designer

### บทบาทและความรับผิดชอบ:

- ออกแบบ User Experience และ User Interface
- สร้าง wireframes, prototypes และ design specs
- ทำ user research และ usability testing
- สร้าง design system และ UI components
- ดูแลความสอดคล้องของ brand และการออกแบบ
- ทำงานร่วมกับ PM เพื่อเข้าใจความต้องการของผู้ใช้

### ความเกี่ยวข้องใน Development Flow:

- **Requirement Analysis**: ทำความเข้าใจ requirement และแปลงเป็น design
- **Design Creation**: สร้าง wireframes, mockups และ interactive prototypes
- **Design Handoff**: ส่งมอบไฟล์ design และ specs ให้ Frontend Developer
- **Design Review**: ตรวจสอบ UI ที่ Frontend พัฒนากับ design เดิม
- **Feedback Handling**: รับ feedback และปรับปรุง design
- **Design QA**: ตรวจสอบความสอดคล้องของ UI ในระบบจริง
- **Design System Maintenance**: ปรับปรุง design system อย่างต่อเนื่อง

---

## 📋 Product Manager (PM)

### บทบาทและความรับผิดชอบ:

- รวบรวมและวิเคราะห์ความต้องการของผู้ใช้และธุรกิจ
- กำหนด product backlog และลำดับความสำคัญของฟีเจอร์
- เขียน user stories และ functional requirements
- ประสานงานระหว่างฝ่ายธุรกิจและทีมพัฒนา
- วิเคราะห์ตลาดและคู่แข่ง
- วางแผนการ release และ roadmap ของผลิตภัณฑ์
- รวบรวมและวิเคราะห์ feedback จากผู้ใช้

### ความเกี่ยวข้องใน Development Flow:

- **Vision Setting**: กำหนดวิสัยทัศน์และเป้าหมายของผลิตภัณฑ์
- **Requirement Gathering**: รวบรวมความต้องการและเขียนเป็น user stories
- **Prioritization**: จัดลำดับความสำคัญของ stories ใน backlog
- **Sprint Planning**: ร่วมกำหนดขอบเขตงานในแต่ละ sprint
- **Acceptance Criteria**: กำหนดเกณฑ์การยอมรับสำหรับแต่ละฟีเจอร์
- **UAT**: ทดสอบและยืนยันว่าฟีเจอร์ตรงตามความต้องการ
- **Product Release**: ตัดสินใจเกี่ยวกับการ release และสื่อสารกับผู้ใช้
- **Feedback Collection**: รวบรวม feedback หลังจาก release เพื่อปรับปรุง

---

## 🔍 Quality Assurance (QA)

### บทบาทและความรับผิดชอบ:

- ออกแบบและเขียน test cases ตาม requirements
- ทดสอบฟีเจอร์ใหม่และฟังก์ชันที่มีอยู่
- ทำ regression testing เมื่อมีการเปลี่ยนแปลงในระบบ
- รายงานและติดตาม bugs
- ทดสอบ usability และ user experience
- ทำงานร่วมกับ Dev เพื่อแก้ไขปัญหาที่พบ
- ทำ automated testing เมื่อเป็นไปได้

### ความเกี่ยวข้องใน Development Flow:

- **Test Planning**: วางแผนการทดสอบตั้งแต่เริ่มโปรเจกต์
- **Test Case Creation**: เขียน test cases ตาม requirements
- **Feature Testing**: ทดสอบฟีเจอร์ที่ Dev ส่งมอบ
- **Bug Reporting**: รายงาน bugs และติดตามการแก้ไข
- **Regression Testing**: ทดสอบระบบโดยรวมก่อนการ release
- **UAT Support**: สนับสนุนการทดสอบ UAT
- **Release Verification**: ตรวจสอบความพร้อมของระบบก่อน deploy ไป production
- **Post-release Testing**: ทดสอบหลังจาก release เพื่อยืนยันความถูกต้อง

---

## 🔄 Flow การทำงานและความเชื่อมโยง

### 1. **Requirement Phase**
- **ผู้จัดการทั่วไป** อนุมัติโปรเจกต์และทรัพยากร
- **PM** รวบรวมความต้องการและเขียน user stories
- **UX/UI Designer** ทำ research และสร้าง wireframes
- **หัวหน้า Dev** ประเมินความเป็นไปได้ทางเทคนิคและทรัพยากรที่ต้องใช้
- **QA** วางแผนการทดสอบเบื้องต้น

### 2. **Design Phase**
- **UX/UI Designer** สร้าง mockups และ prototypes
- **PM** ตรวจสอบว่าตรงตามความต้องการของธุรกิจ
- **หัวหน้า Dev** ออกแบบสถาปัตยกรรมและเลือกเทคโนโลยี
- **Backend Developer** ออกแบบ database schema และ API endpoints
- **Frontend Developer** ให้ feedback เกี่ยวกับความเป็นไปได้ในการพัฒนา UI

### 3. **Development Phase**
- **หัวหน้า Dev** แบ่งงานและมอบหมายงานให้ Dev
- **Backend Developer** พัฒนา API และ services
- **Frontend Developer** พัฒนา UI และเชื่อมต่อกับ API
- **UX/UI Designer** ให้คำแนะนำและตรวจสอบการพัฒนา UI
- **หัวหน้า Dev** ทำ code review และแก้ไขปัญหาทางเทคนิค

### 4. **Testing Phase**
- **Dev** (ทั้ง Backend และ Frontend) ทำ self-testing ก่อนส่ง PR
- **หัวหน้า Dev** review และ approve PRs
- **QA** ทดสอบฟีเจอร์ที่พัฒนาเสร็จใน staging environment
- **PM** ตรวจสอบว่าฟีเจอร์ตรงตาม requirements
- **UX/UI Designer** ตรวจสอบว่า UI ตรงตามการออกแบบ

### 5. **Feedback & Iteration**
- **QA** รายงาน bugs และเขียน bug tickets
- **PM** จัดลำดับความสำคัญของ bugs
- **หัวหน้า Dev** มอบหมายงานการแก้ไข bugs
- **Dev** แก้ไข bugs
- **ผู้จัดการทั่วไป** รับทราบความคืบหน้าและปัญหาสำคัญ

### 6. **Release Phase**
- **หัวหน้า Dev** สร้าง release branch และเตรียม deployment
- **QA** ทำ regression testing
- **PM** ทำ UAT และตัดสินใจว่าพร้อม release หรือไม่
- **ผู้จัดการทั่วไป** อนุมัติการ release ไปยัง production
- **หัวหน้า Dev** ดำเนินการ deploy ไปยัง production

### 7. **Post-Release**
- **QA** ทำ smoke test หลัง deploy
- **PM** รวบรวม user feedback
- **ผู้จัดการทั่วไป** ประเมินความสำเร็จของ release
- **ทุกคน** เข้าร่วม retrospective เพื่อปรับปรุงกระบวนการทำงาน

---

## 📝 RACI Matrix สำหรับกิจกรรมหลัก

| กิจกรรม | GM | Tech Lead | Backend | Frontend | UX/UI | PM | QA |
|---------|:---:|:----------:|:-------:|:--------:|:-----:|:--:|:--:|
| **กำหนดวิสัยทัศน์ผลิตภัณฑ์** | A | C | I | I | C | R | I |
| **รวบรวม Requirements** | I | C | C | C | C | R | C |
| **ออกแบบ UX/UI** | I | C | I | C | R | A | C |
| **ออกแบบสถาปัตยกรรม** | I | R | C | C | I | A | I |
| **พัฒนา Backend** | I | A | R | C | I | I | I |
| **พัฒนา Frontend** | I | A | C | R | C | I | I |
| **Code Review** | I | R | C | C | I | I | I |
| **Testing** | I | C | C | C | C | C | R |
| **Bug Fixing** | I | A | R | R | C | I | C |
| **Release Approval** | A | R | I | I | I | C | C |
| **Post-release Support** | I | A | R | R | I | C | C |

*R - Responsible, A - Accountable, C - Consulted, I - Informed*

---

> 👥 **การทำงานเป็นทีมที่มีประสิทธิภาพคือกุญแจสำคัญสู่ความสำเร็จของโปรเจกต์** 