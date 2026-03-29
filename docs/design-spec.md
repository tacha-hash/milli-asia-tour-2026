# DESIGN SPEC: MILLI ASIA TOUR 2026 🌏🔥

## 1. Layout & Grid System
Designed for maximum impact and visual hierarchy, focusing on the "Bento Box" and "Layered Collage" style.

### **Desktop (1280px+)**
*   **Grid:** 12-Column Grid
*   **Gap:** 24px
*   **Margin:** 80px (Left/Right)
*   **Layout Pattern:** Bento Grid (Asymmetric layout for Hero & Merch)

### **Tablet (768px - 1024px)**
*   **Grid:** 8-Column Grid
*   **Gap:** 16px
*   **Margin:** 40px

### **Mobile (375px - 767px)**
*   **Grid:** 4-Column Grid
*   **Gap:** 12px
*   **Margin:** 20px
*   **Layout Pattern:** Vertical Stack with horizontal scroll for Tour Dates if needed.

---

## 2. Typography Scale
Using a mix of "Heavy Industrial" and "Clean Modern" to reflect MILLI's energy.

| Element | Font | Size (Desktop) | Size (Mobile) | Weight | Line-Height | Case |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Hero Title** | Monument Extended | 120px | 64px | 900 (Black) | 1.0 | Uppercase |
| **Section Header** | Monument Extended | 80px | 48px | 800 (Bold) | 1.1 | Uppercase |
| **Tour City** | Inter | 32px | 24px | 700 (Bold) | 1.2 | Normal |
| **Body / Date** | Inter | 18px | 16px | 400 (Regular) | 1.5 | Normal |
| **Button / Label** | Inter | 14px | 12px | 600 (Semi-Bold) | 1.0 | Uppercase |

**Effects:**
*   **Hero Title:** Apply `mix-blend-mode: difference` or a subtle `text-shadow: 0 0 10px #DA2D40` (Red Glow).
*   **Glitch Effect:** Random `clip-path` and `transform: skew` on hover for titles.

---

## 3. GSAP Animation & Easing
Based on **21st.dev** and **Scottclayton3d**'s smooth interaction patterns.

### **Global Settings**
*   **Default Duration:** 0.8s - 1.2s
*   **Global Ease:** `expo.out` or `power4.out` (Snappy yet smooth)

### **Interaction Rules**
1.  **Entrance Reveal:**
    *   `opacity: 0`, `y: 40`, `skewY: 2` -> `opacity: 1`, `y: 0`, `skewY: 0`.
    *   **Stagger:** 0.1s between elements in a list.
2.  **Scroll Interaction (ScrollTrigger):**
    *   **Hero 3D Model:** `scrub: 1` or `scrub: 1.5` (Lerp effect for 3D rotation).
    *   **Sticky Sections:** Sections should overlap or "unstack" using `pin: true`.
3.  **Hover State (Buttons):**
    *   `scale: 1.05`, `box-shadow: 0 0 20px rgba(218, 45, 64, 0.6)`.

---

## 4. Component Breakdown (Codex-Dot Guide)

### **Hero Section**
*   **Main Visual:** Centered 3D Model (Spline/Three.js) of MILLI's icon or a 3D Firecracker.
*   **Interaction:** 3D object follows mouse move (tilt) and rotates on scroll (Ref: zaBDyEfhrnk).
*   **Background:** Deep Obsidian (#0A0A0A) with animated noise/grain texture.

### **TourRow (Date List)**
*   **Structure:** `Date (Left) | City (Center) | Venue (Center) | Button (Right)`.
*   **Hover Effect:** Background turns Red (#DA2D40) with white text, and an image of the city pops up (Cursor Follower).

### **3D Merch Showcase**
*   **Style:** Bento Box layout.
*   **Interaction:** Clicking a product triggers a "Camera State" transition in Spline to zoom into that specific item.

---

## 5. Color Usage Rules
*   **Primary Background:** `#0A0A0A` (Black)
*   **Secondary Background:** `#1A1A1A` (Dark Grey - for Cards/Bento boxes)
*   **Accent Color:** `#DA2D40` (MILLI Red)
*   **Secondary Accent:** `#C0C0C0` (Metallic Silver - for borders/accents)
*   **Text (Primary):** `#FFFFFF` (White)
*   **Text (Secondary):** `#A0A0A0` (Grey - for descriptions)

---

## 6. Research Synthesis

### **Analysis: 21st.dev (Scottclayton3d Music Portfolio)**
*   **Insight:** Focus on the "Bento Box" structure for information density. Use high-quality 3D assets as focal points within each card.
*   **Implementation:** Apply `backdrop-filter: blur(10px)` on Bento cards for a modern "Glassmorphism" look that contrasts with the aggressive Red/Black theme.

### **Analysis: YouTube Reference (zaBDyEfhrnk)**
*   **Insight:** The "Scroll-to-Transition" technique where 3D scenes change states seamlessly.
*   **Implementation:** Use Spline's "Events" to trigger camera movements when `ScrollTrigger` hits specific markers. The transition must feel "liquid" and continuous.

---

**Prepared by:** Gemini-Dot-Assist (Design Research Agent)
**Report to:** Dot (Design Lead)
**Status:** Ready for Implementation by Codex-Dot
