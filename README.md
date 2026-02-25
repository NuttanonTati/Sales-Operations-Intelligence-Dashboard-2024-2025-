# Sales-Operations-Intelligence-Dashboard-2024-2025-
ระบบวิเคราะห์ข้อมูลการขายเชิงลึกเพื่อตรวจสอบประสิทธิภาพการดำเนินงาน (Operations) และอุดรอยรั่วทางการเงิน (Risk Audit) ท่ามกลางวิกฤตยอดขายที่ลดลงในปี 2025

1. Problem Statement
  ข้อมูลยอดขายจากหลายช่องทางมีความซับซ้อน รหัส SKU ไม่เป็นมาตรฐาน (เช่น รหัส 5. แทนที่จะเป็น 05)

  รายได้ในปี 2025 ตกลงอย่างเห็นได้ชัด (39%) ทำให้ต้องการเครื่องมือที่ช่วยวิเคราะห์ว่าเกิดจากประสิทธิภาพการทำงาน หรือปัจจัยภายนอก

2. Tech Stack & Methodology
  SQL : ใช้ทำ Data Cleaning โดยเฉพาะการใช้ CASE WHEN และ SUBSTR เพื่อจัดระเบียบ SKU และการ UNION ALL ข้อมูล 2 ปีเข้าด้วยกัน

  Google Sheets: สร้าง Interactive Dashboard พร้อมระบบ Slicer เพื่อให้ผู้บริหารเลือกดูข้อมูลตามหมวดหมู่ได้

3. Critical Insights
  Root Cause Analysis: ค้นพบว่ายอดที่ตกลงใน Q1-Q2 ปี 2025 ไม่ได้เกิดจาก Operations (Success Rate ยังสูงที่ 88.2%) แต่มาจากปัจจัยภายนอก:  
    Fraud Impact: ปัญหาความผิดปกติจาก Partner ในจีนช่วงต้นปี
    Supply Chain Disruption: ปัญหาสินค้าขาดสต็อกช่วงตรุษจีน (Chinese New Year)

  Financial Integrity: ตรวจพบออเดอร์ "Completed" ที่มียอดติดลบ (Revenue Outliers) ซึ่งเป็นรอยรั่วสำคัญที่ต้องตรวจสอบนโยบายการคืนเงิน (Refund Policy)

4. Results & Impact
  ระบุ Hero Products (เครื่องพ่นยา) ที่สร้างรายได้กว่า 24.5 ล้านบาท เพื่อการบริหารสต็อกที่แม่นยำ

  Dashboard นี้ช่วยลดเวลาในการกระทบยอดขายและระบุความเสี่ยงได้แบบ Real-time
