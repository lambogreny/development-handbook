# 🚀 วิธีการ Deploy คู่มือบน GitHub

คู่มือนี้จะอธิบายขั้นตอนการ deploy เอกสาร Markdown นี้บน GitHub เพื่อให้สามารถอ่านได้อย่างสะดวกและสวยงาม

## 🔄 ขั้นตอนการ Deploy บน GitHub

### 1. สร้าง Repository ใหม่บน GitHub

1. เข้าสู่ระบบที่ [GitHub](https://github.com)
2. คลิกที่ปุ่ม "New" หรือ "+" ที่มุมขวาบนของหน้าจอ และเลือก "New repository"
3. ตั้งชื่อ repository เช่น `dev-team-handbook` หรือ `development-guidelines`
4. เพิ่มคำอธิบายสั้นๆ เช่น "คู่มือการพัฒนาและการบริหารทีม"
5. เลือก "Public" หากต้องการให้ทุกคนสามารถเข้าถึงได้ หรือ "Private" หากต้องการจำกัดการเข้าถึง
6. คลิก "Create repository"

### 2. Upload ไฟล์ไปยัง GitHub

**วิธีที่ 1: Upload ผ่าน Git Command Line**

1. เปิด Terminal หรือ Command Prompt
2. นำเข้าสู่โฟลเดอร์ที่เก็บไฟล์ Markdown ทั้งหมด:
   ```
   cd /path/to/your/markdown-files
   ```

3. เริ่มต้น Git repository ในโฟลเดอร์นั้น:
   ```
   git init
   ```

4. เพิ่มไฟล์ทั้งหมดเข้าสู่ staging area:
   ```
   git add .
   ```

5. Commit ไฟล์:
   ```
   git commit -m "เพิ่มคู่มือการพัฒนาซอฟต์แวร์และการบริหารทีม"
   ```

6. เพิ่ม remote repository ที่คุณสร้างบน GitHub:
   ```
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
   ```

7. Push ไฟล์ไปยัง GitHub:
   ```
   git push -u origin main
   ```
   (หรือ `git push -u origin master` หากใช้ branch master)

**วิธีที่ 2: Upload ผ่าน GitHub Web Interface**

1. ไปที่ repository ที่คุณสร้างบน GitHub
2. คลิกที่ปุ่ม "Add file" และเลือก "Upload files"
3. ลากไฟล์และโฟลเดอร์ทั้งหมดลงในพื้นที่ที่กำหนด
4. เพิ่มข้อความอธิบายการ commit
5. คลิก "Commit changes"

### 3. ตั้งค่า GitHub Pages (ทางเลือก)

หากต้องการให้เอกสารของคุณมีหน้าตาสวยงามมากขึ้น คุณสามารถใช้ GitHub Pages:

1. ไปที่ repository ของคุณบน GitHub
2. คลิกที่ "Settings"
3. เลื่อนลงไปที่ส่วน "GitHub Pages"
4. ที่ "Source" เลือก branch ที่คุณต้องการใช้ (เช่น main)
5. เลือก folder "/" (root) หรือ "/docs" ขึ้นอยู่กับโครงสร้างของคุณ
6. เลือก theme ที่คุณต้องการ (ทางเลือก)
7. คลิก "Save"

หลังจากตั้งค่าแล้ว คุณจะได้รับ URL ที่สามารถเข้าถึงเอกสารของคุณได้ เช่น `https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME/`

### 4. เพิ่ม Collaborators (หากเป็น Private Repository)

หากคุณสร้าง private repository และต้องการให้ทีมของคุณเข้าถึงได้:

1. ไปที่ repository ของคุณบน GitHub
2. คลิกที่ "Settings"
3. เลือก "Manage access" จากเมนูด้านซ้าย
4. คลิก "Invite a collaborator"
5. ป้อนชื่อผู้ใช้หรืออีเมลของคนที่คุณต้องการเชิญ
6. คลิก "Add [username] to [repository]"

## 📋 การใช้งานเอกสารบน GitHub

### การนำทางในเอกสาร

เมื่อ deploy เอกสารบน GitHub แล้ว:

1. เอกสาร README.md จะแสดงเป็นหน้าแรกของ repository อัตโนมัติ
2. ลิงก์ที่อยู่ใน README.md จะสามารถคลิกเพื่อนำทางไปยังไฟล์อื่นๆ ได้
3. ผู้อ่านสามารถใช้เมนูไฟล์ด้านบนเพื่อเรียกดูไฟล์ต่างๆ ได้โดยตรง

### การอัปเดตเอกสาร

เมื่อต้องการอัปเดตเอกสาร:

1. ทำการแก้ไขไฟล์ในเครื่องของคุณ
2. ใช้คำสั่ง Git เพื่อ commit และ push การเปลี่ยนแปลง:
   ```
   git add .
   git commit -m "อัปเดตเอกสาร [ระบุเอกสารที่แก้ไข]"
   git push
   ```

หรือถ้าต้องการแก้ไขเล็กน้อย คุณสามารถแก้ไขไฟล์โดยตรงบน GitHub:
1. ไปที่ไฟล์ที่ต้องการแก้ไข
2. คลิกที่ไอคอนดินสอ (Edit this file)
3. ทำการแก้ไข
4. คลิก "Commit changes"

## 🌟 เทคนิคเพิ่มเติม

### การใช้ GitHub Wiki

นอกจากการใช้ไฟล์ Markdown ใน repository แล้ว คุณยังสามารถใช้ GitHub Wiki:

1. ไปที่ repository ของคุณ
2. คลิกที่แท็บ "Wiki"
3. คลิก "Create the first page"
4. สร้างเนื้อหาโดยใช้ Markdown
5. คลิก "Save page"

Wiki เหมาะสำหรับเอกสารที่มีการเชื่อมโยงกันและมีการแก้ไขบ่อย

### การใช้ GitHub Issues สำหรับการรวบรวม feedback

คุณสามารถใช้ GitHub Issues เพื่อรับ feedback เกี่ยวกับเอกสาร:

1. ไปที่ repository ของคุณ
2. คลิกที่แท็บ "Issues"
3. ตั้งค่าป้ายกำกับ (labels) สำหรับประเภทของ feedback เช่น "documentation", "suggestion", "correction"
4. สนับสนุนให้ทีมสร้าง Issue เมื่อพบข้อผิดพลาดหรือมีข้อเสนอแนะ

## 📱 การเข้าถึงบนอุปกรณ์มือถือ

เอกสาร Markdown บน GitHub สามารถอ่านได้อย่างสะดวกบนอุปกรณ์มือถือ ไม่จำเป็นต้องทำอะไรเพิ่มเติม เพียงแค่ส่ง URL ของ repository หรือ GitHub Pages ให้กับทีมของคุณ

---

> 🔗 หากมีคำถามหรือต้องการความช่วยเหลือเพิ่มเติมเกี่ยวกับการ deploy เอกสารนี้บน GitHub กรุณาติดต่อ [ชื่อผู้ดูแล] 