# SC 133 General Physics 1 (ฟิสิกส์ 1) - Formula Cheat Sheet
> **คณะวิศวกรรมศาสตร์ มหาวิทยาลัยธรรมศาสตร์**  
> จัดทำโดย: **ธนภรณ์ นพรัตน์ (Thanaporn Nopparat)** • ภาควิชาวิศวกรรมโยธา คณะวิศวกรรมศาสตร์ มหาวิทยาลัยธรรมศาสตร์  
> มาตรฐานการแสดงผลและดีไซน์: ถอดแบบ 100% จากสถาปัตยกรรม [CE272](https://thanakornnopp-dev.github.io/CE272/)

[![Live Website](https://img.shields.io/badge/🌍_Live_Website-คลิกเปิดแผ่นสรุป_A5_หน้าเดียวได้ทันที-success?style=for-the-badge&logo=googlechrome&logoColor=white)](https://thanakornnopp-dev.github.io/sc133-physics1/)
[![Full Study Portal](https://img.shields.io/badge/📖_Full_Portal-คลิกเปิดชีทสรุปสูตรฉบับเต็ม-blue?style=for-the-badge&logo=safari&logoColor=white)](https://thanakornnopp-dev.github.io/sc133-physics1/sc133_formula_sheet_full.html)
[![LaTeX Source](https://img.shields.io/badge/📄_LaTeX_Source-ดาวน์โหลดไฟล์_.tex_สำหรับ_Overleaf-darkgreen?style=for-the-badge&logo=latex)](https://github.com/thanakornnopp-dev/sc133-physics1/blob/main/sc133_cheat_sheet_a5.tex)

---

## 🌐 ลิงก์เข้าชมเว็บสรุปสูตรออนไลน์ (Live Links)

👉 **1. แผ่นสรุปสูตร A5 หน้าเดียว (One-Page A5 Printable Sheet):**  
[https://thanakornnopp-dev.github.io/sc133-physics1/](https://thanakornnopp-dev.github.io/sc133-physics1/)  
*(ออกแบบสัดส่วน 148 × 210 mm พอดี 1 หน้ากระดาษ A5 เป๊ะ มีปุ่มกด Print สั่งพิมพ์ออก PDF หรือจดตามได้ทันที)*

👉 **2. พอร์ทัลสรุปสูตรฉบับละเอียด (Full Interactive Portal):**  
[https://thanakornnopp-dev.github.io/sc133-physics1/sc133_formula_sheet_full.html](https://thanakornnopp-dev.github.io/sc133-physics1/sc133_formula_sheet_full.html)  
*(มีตารางสูตรภาพรวม, การ์ดสูตรเจาะลึก 3 บท, และสลับโหมดมืด/สว่าง)*

👉 **3. ซอร์สโค้ด LaTeX ฉบับ Overleaf-Ready:**  
[https://github.com/thanakornnopp-dev/sc133-physics1/blob/main/sc133_cheat_sheet_a5.tex](https://github.com/thanakornnopp-dev/sc133-physics1/blob/main/sc133_cheat_sheet_a5.tex)  
*(เขียนด้วยคำสั่ง LaTeX มาตรฐาน `amsmath`, `geometry[a5paper]`, `tcolorbox`, `multicol` จัดหน้า A5 หน้าเดียวสมบูรณ์แบบ)*

---

## 📖 สรุปเนื้อหาและสมการควบคุม 3 บทหลัก

### 1. บทที่ 5: การแกว่งกวัด (Oscillatory Motion & SHM)
* **คาบและความถี่:** $T = \dfrac{1}{f} = \dfrac{2\pi}{\omega}, \quad \omega = 2\pi f\,\left[\text{rad/s}\right]$
* **การกระจัด:** $x(t) = A\sin(\omega t + \phi) \quad (x=0 \to v_{\max})$
* **ความเร็ว:** $v(t) = \omega A\cos(\omega t + \phi) = \pm\omega\sqrt{A^2 - x^2}$
* **ความเร่ง:** $a(t) = -\omega^2 A\sin(\omega t + \phi) = -\omega^2 x \quad (x=\pm A \to a_{\max})$
* **มวลติดสปริง:** $\omega = \sqrt{\dfrac{k}{m}}, \quad T = 2\pi\sqrt{\dfrac{m}{k}}$
* **พลังงานกลรวม:** $E = \dfrac{1}{2}kA^2 = \dfrac{1}{2}mv^2 + \dfrac{1}{2}kx^2 = \text{คงที่}$
* **ลูกตุ้มอย่างง่าย (Simple):** $T = 2\pi\sqrt{\dfrac{L}{g}} \quad (\text{ไม่ขึ้นกับมวล } m)$
* **ลูกตุ้มกายภาพ (Physical):** $T = 2\pi\sqrt{\dfrac{I}{mgd}} \quad (d: \text{จุดหมุน } O \to \text{CM})$
* **ลูกตุ้มชนิดบิด (Torsion):** $\tau = -\kappa\theta, \quad T = 2\pi\sqrt{\dfrac{I}{\kappa}}$
* **การแกว่งกวัดแบบหน่วง:** $A(t) = A_0 e^{-\gamma t} \quad \left(\gamma = \dfrac{b}{2m}, \; \omega' = \sqrt{\omega_0^2 - \gamma^2}\right)$
  * หน่วงเกิน ($\gamma > \omega_0$), หน่วงวิกฤต ($\gamma = \omega_0$), หน่วงน้อย ($\gamma < \omega_0$)
* **การสั่นพ้อง (Resonance):** $\omega_f = \omega_0 \implies A \to \text{สูงสุด}$

---

### 2. บทที่ 6: คลื่นและคลื่นเสียง (Wave Motion & Sound Waves)
* **อัตราเร็วคลื่น:** $v = f\lambda = \dfrac{\omega}{k}, \quad k = \dfrac{2\pi}{\lambda}\,\left[\text{rad/m}\right]$
* **ฟังก์ชันคลื่น:** $y(x,t) = A\sin(kx \mp \omega t) \quad [-\text{ขวา}, +\text{ซ้าย}]$
* **อัตราเร็วในตัวกลาง:**
  * ในเส้นเชือก: $v = \sqrt{\dfrac{T}{\mu}} \quad \left(\mu = \dfrac{m}{L}\right)$
  * ในน้ำตื้น: $v = \sqrt{gd}$
  * ในของแข็ง: $v = \sqrt{\dfrac{Y}{\rho}}$
  * ในของไหล: $v = \sqrt{\dfrac{B}{\rho}}$
  * เสียงในอากาศ: $v_T = 331 + 0.6T_C\,\left[\text{m/s}\right] \quad (T_C \text{ หน่วย } ^\circ\text{C})$
* **กฎของสเนลล์ (Snell's Law):** $\dfrac{\sin\theta_1}{\sin\theta_2} = \dfrac{v_1}{v_2} = \dfrac{\lambda_1}{\lambda_2} = \dfrac{n_2}{n_1} \quad (f \text{ คงที่เสมอ})$
* **การแทรกสอด (เฟสตรงกัน):**
  * แนวปฏิบัพ (เสริม): $d\sin\theta = n\lambda \quad (n=0,1,2,\dots)$
  * แนวบัพ (หักล้าง): $d\sin\theta = \left(n - \dfrac{1}{2}\right)\lambda \quad (n=1,2,\dots)$
* **คลื่นนิ่งเชือก 2 ปลาย / ท่อเปิด 2 ด้าน:** $f_n = \dfrac{nv}{2L} = n f_1 \quad (n = 1, 2, 3, \dots \text{มีครบทุกฮาร์มอนิก})$
* **คลื่นนิ่งท่อปิด 1 ด้าน:** $f_n = \dfrac{nv}{4L} = n f_1 \quad (n = 1, 3, 5, \dots \mathbf{\text{ คี่เท่านั้น!}})$
* **หลอดเรโซแนนซ์:** $L_2 - L_1 = \dfrac{\lambda}{2} \implies v = 2(L_2 - L_1)f$
* **ความเข้ม \& ระดับเสียง:** $I = \dfrac{P}{4\pi R^2}, \quad \beta = 10\log_{10}\left(\dfrac{I}{10^{-12}}\right) \quad [\text{dB}]$
* **บีตส์ (Beats):** $f_{\text{beat}} = |f_1 - f_2| \quad (\text{ติดขี้ผึ้ง } m \uparrow \implies f \downarrow)$
* **ดอปเปลอร์ (Doppler Effect):** $f' = f\left(\dfrac{v \pm v_o}{v \mp v_s}\right) \quad \left[\dfrac{\text{ผู้สังเกต } (+ \text{เข้า}, - \text{หนี})}{\text{แหล่งกำเนิด } (- \text{เข้า}, + \text{หนี})}\right]$
* **คลื่นกระแทก:** $\sin\theta = \dfrac{v}{v_s}, \quad M = \dfrac{v_s}{v} = \dfrac{1}{\sin\theta}$

---

### 3. บทที่ 7: สมบัติเชิงกลและกลศาสตร์ของไหล (Properties of Matter & Fluids)
* **ความเค้น & ความเครียด:** $\sigma = \dfrac{F}{A}\,\left[\text{Pa}\right], \quad e = \dfrac{\Delta L}{L_0}, \quad \gamma \approx \theta = \dfrac{a}{h}$
* **มอดูลัสความยืดหยุ่น:** $Y = \dfrac{F L_0}{A \Delta L}, \quad S = \dfrac{F/A}{\gamma}, \quad B = -\dfrac{\Delta P}{\Delta V / V_0}$
* **ความดันของเหลว:** $P_G = \rho gh, \quad P_{\text{abs}} = P_{\text{atm}} + \rho gh \quad (P_{\text{atm}} = 1.013 \times 10^5\,\text{Pa})$
* **หลอดตัวยู (Manometer):** $P_{\text{ซ้าย}} = P_{\text{ขวา}} \implies \rho_1 h_1 = \rho_2 h_2$
* **กฎของปาสคาล & แม่แรงไฮดรอลิกส์:** $\dfrac{F_1}{A_1} = \dfrac{F_2}{A_2} \implies F_2 = F_1\left(\dfrac{d_2}{d_1}\right)^2$
* **คานโยก:** $F_{\text{มือ}} \cdot L = F_1 \cdot l \implies F_1 = F_{\text{มือ}}\left(\dfrac{L}{l}\right)$
* **แรงลอยตัว (Archimedes):** $F_B = \rho_{\text{fluid}} g V_{\text{sub}}, \quad T_{\text{ชั่งในน้ำ}} = mg - F_B$
* **แรงตึงผิว ($\gamma$):** ฟิล์มตรง $\gamma = \dfrac{F}{2l}$, ห่วงกลม $\gamma = \dfrac{F}{4\pi r}$
* **สมการความต่อเนื่อง:** $A_1 v_1 = A_2 v_2 = Q\,\left[\text{m}^3/\text{s}\right] \quad (\rho \text{ คงที่})$
* **สมการแบร์นูลลี:** $P_1 + \dfrac{1}{2}\rho v_1^2 + \rho gh_1 = P_2 + \dfrac{1}{2}\rho v_2^2 + \rho gh_2$
* **ท่อเวนจูรีมิเตอร์:** $v_1 = \sqrt{\dfrac{2gh}{(A_1/A_2)^2 - 1}}$
* **แรงยกปีกเครื่องบิน:** $F_{\text{lift}} = \dfrac{1}{2}\rho(v_{\text{บน}}^2 - v_{\text{ล่าง}}^2)A$
* **รูรั่วข้างถัง (Torricelli):** $v = \sqrt{2gh}, \quad x_{\text{ตก}} = 2\sqrt{h(H-h)}$
* **กฎของสโตกส์ & ความเร็วปลาย:** $F_f = 6\pi\eta R v \implies v_t = \dfrac{2}{9}\dfrac{R^2 g}{\eta}(\rho_{\text{กลม}} - \rho_{\text{ไหล}})$

---

## ⚡ ข้อควรระวังในห้องสอบ (Exam Traps Checklist)
1. **ตรีโกณมิติ SHM:** โหมดเครื่องคิดเลขต้องตั้งเป็น **`RAD`** เสมอ
2. **ฮาร์มอนิกท่อปิด 1 ด้าน:** มีเฉพาะฮาร์มอนิก **เลขคี่ ($n=1,3,5$)** ห้ามใช้ $n=2$
3. **แม่แรงไฮดรอลิกส์:** หากโจทย์ให้เส้นผ่านศูนย์กลางมา **ต้องยกกำลังสอง** $\left(\frac{d_2}{d_1}\right)^2$
4. **แรงลอยตัว:** ใช้ความหนาแน่น $\rho$ ของ **"ของเหลว"** และปริมาตร $V$ **"เฉพาะส่วนที่จม"** เท่านั้น
5. **กฎของสโตกส์:** ตัวแปร $R$ คือ **รัศมี** หากโจทย์ให้ $D$ ต้องนำมาหาร 2 ก่อนคำนวณเสมอ
