# SC 133 General Physics 1 (ฟิสิกส์ 1) - Formula Cheat Sheet
> **คณะวิศวกรรมศาสตร์ มหาวิทยาลัยธรรมศาสตร์**  
> จัดทำโดย: ธนภรณ์ นพรัตน์ (Thanaporn Nopparat)  
> ถอดแบบสถาปัตยกรรมและดีไซน์จาก: [CE 272 Study Portal](https://github.com/thanakornnopp-dev/CE272)

---

## 📌 สรุปสูตรกระดาษ A5 หน้าเดียว (One-Page A5 Formula Sheet)
เอกสารชุดนี้จัดทำขึ้นสำหรับสรุปสูตรฟิสิกส์ 3 บทหลัก (บทที่ 5 การแกว่งกวัด, บทที่ 6 คลื่นและเสียง, บทที่ 7 สมบัติเชิงกลและของไหล) โดยเน้นความกระชับ สามารถจดด้วยมือลงบนกระดาษขนาด **A5 หน้าเดียว** ได้พอดี หรือสั่งพิมพ์ผ่านหน้าเว็บได้ทันที

### ไฟล์ภายใน Repository:
1. `sc133_cheat_sheet_a5.tex` : ซอร์สโค้ด LaTeX ฉบับเต็ม (Overleaf-ready) จัดหน้ากระดาษ A5 แบบ 2 คอลัมน์ ออกแบบตามมาตรฐาน `engineering-latex-format`
2. `index.html` / `sc133_cheat_sheet_a5.html` : เว็บแอปสรุปสูตร A5 หน้าเดียว พร้อมปุ่มสั่งพิมพ์ (Print-Ready) และ KaTeX
3. `sc133_formula_sheet_full.html` : เว็บพอร์ทัลสรุปสูตรฉบับเต็ม พร้อมการ์ดสูตรและตารางวิเคราะห์

---

## 📐 โครงสร้างสูตรหลัก (Master Equations)

### บทที่ 5: การเคลื่อนที่แบบแกว่งกวัด (Oscillatory Motion & SHM)
- **คาบและความถี่:** $T = \dfrac{1}{f} = \dfrac{2\pi}{\omega}, \quad \omega = 2\pi f\,\left[\text{rad/s}\right]$
- **การกระจัด:** $x(t) = A\sin(\omega t + \phi)$
- **ความเร็ว:** $v(t) = \omega A\cos(\omega t + \phi) = \pm\omega\sqrt{A^2 - x^2} \implies v_{\max} = \omega A$ (ที่ $x=0$)
- **ความเร่ง:** $a(t) = -\omega^2 x \implies a_{\max} = \omega^2 A$ (ที่ $x=\pm A$)
- **มวลติดสปริง:** $\omega = \sqrt{\dfrac{k}{m}}, \quad T = 2\pi\sqrt{\dfrac{m}{k}}$
- **พลังงานกลรวม:** $E = \dfrac{1}{2}kA^2 = \dfrac{1}{2}mv^2 + \dfrac{1}{2}kx^2 = \text{คงที่}$
- **ลูกตุ้มอย่างง่าย (Simple Pendulum):** $T = 2\pi\sqrt{\dfrac{L}{g}}$ (ไม่ขึ้นกับมวล $m$)
- **ลูกตุ้มกายภาพ (Physical Pendulum):** $T = 2\pi\sqrt{\dfrac{I}{mgd}}$ ($d$ คือระยะจากจุดหมุนถึง CM)
- **ลูกตุ้มชนิดบิด (Torsion Pendulum):** $\tau = -\kappa\theta, \quad T = 2\pi\sqrt{\dfrac{I}{\kappa}}$
- **การแกว่งกวัดแบบหน่วง (Damped Motion):** $A(t) = A_0 e^{-\gamma t}$ โดย $\gamma = \dfrac{b}{2m}, \quad \omega' = \sqrt{\omega_0^2 - \gamma^2}$

### บทที่ 6: การเคลื่อนที่แบบคลื่นและคลื่นเสียง (Wave Motion & Sound Waves)
- **อัตราเร็วคลื่น:** $v = f\lambda = \dfrac{\omega}{k}, \quad k = \dfrac{2\pi}{\lambda}$
- **ฟังก์ชันคลื่น:** $y(x,t) = A\sin(kx \mp \omega t)$ ($- \omega t$ ไปทางขวา, $+ \omega t$ ไปทางซ้าย)
- **อัตราเร็วในตัวกลาง:**
  - เชือกตึง: $v = \sqrt{\dfrac{T}{\mu}} \quad \left(\mu = \dfrac{m}{L}\right)$
  - น้ำตื้น: $v = \sqrt{gd}$
  - ของแข็ง: $v = \sqrt{\dfrac{Y}{\rho}}$
  - ของไหล: $v = \sqrt{\dfrac{B}{\rho}}$
  - เสียงในอากาศ: $v_T = 331 + 0.6T_C\,\left[\text{m/s}\right]$
- **กฎของสเนลล์ (Snell's Law):** $\dfrac{\sin\theta_1}{\sin\theta_2} = \dfrac{v_1}{v_2} = \dfrac{\lambda_1}{\lambda_2} = \dfrac{n_2}{n_1}$ ($f$ คงที่เสมอ)
- **การแทรกสอด (เฟสตรงกัน):**
  - แนวปฏิบัพ (เสริม): $d\sin\theta = n\lambda \quad (n=0,1,2,\dots)$
  - แนวบัพ (หักล้าง): $d\sin\theta = \left(n - \dfrac{1}{2}\right)\lambda \quad (n=1,2,\dots)$
- **คลื่นนิ่งในเชือก 2 ปลาย / ท่อเปิด 2 ด้าน:** $f_n = \dfrac{nv}{2L} = n f_1 \quad (n=1,2,3,\dots)$
- **คลื่นนิ่งในท่อปิด 1 ด้าน:** $f_n = \dfrac{nv}{4L} = n f_1 \quad (n=1,3,5,\dots \text{คี่เท่านั้น!})$
- **ความเข้ม & ระดับความเข้มเสียง:** $I = \dfrac{P}{4\pi R^2}, \quad \beta = 10\log_{10}\left(\dfrac{I}{10^{-12}}\right)$
- **บีตส์ (Beats):** $f_{\text{beat}} = |f_1 - f_2|$
- **ดอปเปลอร์ (Doppler Effect):** $f' = f\left(\dfrac{v \pm v_o}{v \mp v_s}\right)$
- **คลื่นกระแทก:** $\sin\theta = \dfrac{v}{v_s}, \quad M = \dfrac{v_s}{v} = \dfrac{1}{\sin\theta}$

### บทที่ 7: สมบัติเชิงกลของสารและกลศาสตร์ของไหล (Properties of Matter & Fluids)
- **ความเค้น & ความเครียด:** $\sigma = \dfrac{F}{A}, \quad e = \dfrac{\Delta L}{L_0}, \quad \gamma \approx \theta = \dfrac{a}{h}$
- **มอดูลัสความยืดหยุ่น:** $Y = \dfrac{F L_0}{A \Delta L}, \quad S = \dfrac{F/A}{\gamma}, \quad B = -\dfrac{\Delta P}{\Delta V / V_0}$
- **ความดันของเหลว:** $P_G = \rho gh, \quad P_{\text{abs}} = P_{\text{atm}} + \rho gh \quad (P_{\text{atm}} = 1.013 \times 10^5\,\text{Pa})$
- **กฎของปาสคาล & แม่แรงไฮดรอลิกส์:** $\dfrac{F_1}{A_1} = \dfrac{F_2}{A_2} \implies F_2 = F_1\left(\dfrac{d_2}{d_1}\right)^2$
- **คานโยก:** $F_{\text{hand}} \cdot L = F_1 \cdot l \implies F_1 = F_{\text{hand}}\left(\dfrac{L}{l}\right)$
- **แรงลอยตัว (Archimedes):** $F_B = \rho_{\text{fluid}} g V_{\text{sub}}, \quad T = mg - F_B$
- **แรงตึงผิว:** ฟิล์มตรง $\gamma = \dfrac{F}{2l}$, ห่วงกลม $\gamma = \dfrac{F}{4\pi r}$
- **สมการความต่อเนื่อง:** $A_1 v_1 = A_2 v_2 = Q\,\left[\text{m}^3/\text{s}\right]$
- **สมการแบร์นูลลี:** $P_1 + \dfrac{1}{2}\rho v_1^2 + \rho gh_1 = P_2 + \dfrac{1}{2}\rho v_2^2 + \rho gh_2$
- **เวนจูรีมิเตอร์:** $v_1 = \sqrt{\dfrac{2gh}{(A_1/A_2)^2 - 1}}$
- **แรงยกปีกเครื่องบิน:** $F_{\text{lift}} = \dfrac{1}{2}\rho(v_{\text{top}}^2 - v_{\text{bottom}}^2)A$
- **รูรั่วข้างถัง (Torricelli):** $v = \sqrt{2gh}, \quad x_{\text{ตก}} = 2\sqrt{h(H-h)}$
- **กฎของสโตกส์ & ความเร็วปลาย:** $F_f = 6\pi\eta R v \implies v_t = \dfrac{2}{9}\dfrac{R^2 g}{\eta}(\rho_{\text{solid}} - \rho_{\text{fluid}})$

---

## ⚡ ข้อควรระวังในการสอบ (Exam Traps)
1. **มุมตรีโกณมิติ SHM:** ต้องตั้งโหมดเครื่องคิดเลขเป็น **`RAD`** เสมอ
2. **ฮาร์มอนิกท่อปิด 1 ด้าน:** มีเฉพาะเลขคี่ ($n=1,3,5$) ห้ามใช้ $n=2$ เด็ดขาด
3. **แม่แรงไฮดรอลิกส์:** หากโจทย์ให้ขนาดเส้นผ่านศูนย์กลางมา ต้อง **ยกกำลังสอง** $\left(\frac{d_2}{d_1}\right)^2$
4. **แรงลอยตัว $F_B$:** ใช้ความหนาแน่น $\rho$ ของ **ของเหลว** และปริมาตร $V$ **เฉพาะส่วนที่จม** เท่านั้น
5. **กฎของสโตกส์:** ตัวแปร $R$ ในสูตรคือ **รัศมี** หากโจทย์ให้ $D$ ต้องหาร 2 ก่อนเสมอ
