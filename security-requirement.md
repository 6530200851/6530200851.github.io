# 🔒 OWASP Application Security Verification Standard

## 📂 V12.5.2 File Download  
✅ **ตรวจสอบให้แน่ใจว่าคำขอโดยตรงไปยังไฟล์ที่อัปโหลดจะไม่ถูกดำเนินการเป็นเนื้อหา HTML/JavaScript**  

---

## 🎯 สรุป  
📌 **ป้องกันไฟล์ที่อัปโหลดไม่ให้รันเป็น HTML/JavaScript**  

### 🔹 ตัวอย่างแนวทางป้องกัน  
- กำหนดค่า **Content-Type** เป็น `application/octet-stream` สำหรับไฟล์ที่ดาวน์โหลด  
- ป้องกัน **MIME sniffing** โดยใช้ `X-Content-Type-Options: nosniff`  
- หลีกเลี่ยงการเก็บไฟล์ที่อัปโหลดในโฟลเดอร์ที่เว็บเซิร์ฟเวอร์สามารถรันโค้ดได้  
- ใช้ **sandboxing** หรือ Content Security Policy (CSP) เพื่อลดความเสี่ยง  

---

👨‍💻 **Contributor**: [Supanimit Nilchawee](https://6530200517.github.io/security-requirement)  

📎 **Reference**: [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/)  


