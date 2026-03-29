# MILLI ASIA TOUR: Design Research Report

## 1. Concert Tour Landing Page Analysis
จากการวิเคราะห์หน้า Landing Page ของศิลปินระดับโลก พบ Design Patterns ที่น่าสนใจดังนี้:

### **Billie Eilish (Aesthetic: Lo-Fi Abyss)**
*   **Design Pattern:** เน้นความมืดมน (Dark Mode) ผสมผสานกับ Analog Textures และ Glitch effects.
*   **Typography:** ใช้ Font ที่มีความขัดแย้งสูง (High Contrast) เช่น Serif ที่ดูหรูหราตัดกับ Sans-Serif แบบ Minimalist หรือลายมือ (Handwriting).
*   **Interaction:** มีการใช้ Fluid movement เหมือนน้ำ และการจัดวาง Layout ที่ดูเหมือนงาน Collage.

### **Blackpink (Aesthetic: Dual Identity)**
*   **Design Pattern:** การใช้ธีมคู่ขนาน (Contrast) เช่น ความหวานของสีชมพู (Balletcore) ตัดกับความดุดันของสีดำ/เงิน (Military-Chic).
*   **Visual Elements:** ใช้ภาพถ่ายแฟชั่นคุณภาพสูง (High-Fashion Photography) เป็นตัวชูโรง ผสมกับเส้นสายแบบ Industrial/Metallic.
*   **Layout:** มักใช้ Grid ที่สะอาดตาแต่มีลูกเล่นการซ้อนทับ (Layering) ของรูปภาพและข้อความ.

### **BTS (Aesthetic: Layered Persona)**
*   **Design Pattern:** เน้นการเล่าเรื่อง (Storytelling) ผ่านสัญลักษณ์ (Symbols) และการใช้สีที่สื่อถึง "ตัวตน" ที่หลากหลาย.
*   **Typography:** สมาชิกแต่ละคนอาจมีสไตล์ฟอนต์ที่ต่างกันเพื่อสะท้อนบุคลิก (e.g., Serif สำหรับความเป็นทางการ, Sans-Serif สำหรับความทันสมัย).
*   **Space:** การใช้ White Space (หรือ Negative Space) อย่างชาญฉลาดเพื่อให้องค์ประกอบสำคัญดูโดดเด่นและมีพลัง.

---

## 2. 3D Merchandise & Scroll Animation Techniques
เทคนิคที่ใช้ในเว็บระดับโลกอย่าง Apple และ Nike เพื่อสร้างประสบการณ์ที่น่าตื่นเต้น:

### **Apple-Style "Flip-Book" Scroll (Image Sequence)**
*   **Technique:** การใช้ Canvas + GSAP (GreenSock Animation Platform) เพื่อเล่นลำดับภาพนิ่ง (Image Sequence) ตามความเร็วการ Scroll.
*   **Effect:** ให้ความรู้สึกเหมือนกำลังหมุนวัตถุ 3D จริงๆ ที่มีความลื่นไหลและตอบสนองต่อมือผู้ใช้งานได้อย่างแม่นยำ (Frame-perfect scrubbing).

### **Nike 3D Showcase (Three.js + GLTF)**
*   **Technique:** การ Render โมเดล 3D จริงๆ บน Browser โดยใช้ Three.js.
*   **Scroll Interaction:**
    *   **Rotation:** เมื่อ Scroll วัตถุจะหมุนเพื่อโชว์มุมมองต่างๆ.
    *   **Exploded View:** เมื่อถึงจุดที่กำหนด ชิ้นส่วนของสินค้าจะกระจายออก (Deconstructed) เพื่อโชว์วัสดุภายใน.
    *   **Floating Effect:** การเพิ่ม Micro-interactions เช่น วัตถุลอยขึ้นลงเล็กน้อย (Sine-wave movement) เพื่อให้ดู "มีชีวิต".

### **Parallax Typography**
*   **Effect:** การให้ข้อความและวัตถุ 3D เคลื่อนที่ด้วยความเร็วที่ต่างกัน (Depth perception) สร้างมิติให้กับหน้าเว็บ.

---

## 3. Color Palette Analysis: MILLI ASIA TOUR (Red, Black, White)
วิเคราะห์จาก Key Visual (KV) ของ MILLI ที่มีความเป็น "Firestarter" และ "Rebellious":

### **Core Palette:**
*   **Power Red (#DA2D40):** สีหลักที่สื่อถึงพลัง ความร้อนแรง (Fire) และความมั่นใจ.
*   **Obsidian Black (#0A0A0A):** ให้ความรู้สึกดุดัน มั่นคง และเป็นพื้นหลังที่ขับเน้นสีอื่นได้ดีที่สุด.
*   **Pure White (#FFFFFF):** ใช้สำหรับ Typography และเส้นสายที่ต้องการความคมชัด (Crispness).

### **Recommended Extended Palette (เพื่อเพิ่มมิติ):**
*   **Voltage Gold (#FAC553):** สีเหลืองทอง/ส้ม เพื่อสื่อถึง "Mango Sticky Rice" โมเมนต์ และเพิ่มความ Y2K/Street energy.
*   **Dark Plum (#210D19):** สีม่วงเข้มเกือบดำ สำหรับใช้ในส่วน Shadow หรือ Background ที่ต้องการความลึกมากกว่าสีดำล้วน.
*   **Cyber Silver (#C0C0C0):** สีเงิน Metallic เพื่อเพิ่มกลิ่นอายความล้ำสมัย (Futuristic/Industrial).

### **Design Suggestion for MILLI:**
*   ใช้ **Glitch Effect** บนตัวอักษรสีขาวบนพื้นหลังสีดำ.
*   ใช้ **Red Glow (Neon)** รอบๆ วัตถุ 3D หรือภาพถ่ายของ MILLI เพื่อสร้างบรรยากาศคอนเสิร์ต.
*   ผสมผสาน **Thai Typography** ที่มีความโค้งมนตัดกับเส้นสายที่เป็นเหลี่ยมคมแบบ Electronic.
