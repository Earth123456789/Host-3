# Kernel

### Kernel คือ อะไร ?
>ระบบปฏิบัติการที่มีหน้าที่จัดการทรัพยากรของระบบและจัดการกับการประมวลผล โดยจะเป็นตัวกลางที่มีหน้าที่ติดต่อระหว่าง Software กับ Hardware
  
* ใส่รูปตรงนี้  

### หน้าที่ของ Kernel
>Kernel มีหน้าที่เป็นส่วนช่วยติดต่อสื่อสารระหว่างแอปพลิเคชั่นและฮาร์ดแวร์แบบ low-level services มีอยู่ 4 อย่างได้แก่

1. การจัดการการใช้งานหน่วยความจำ คอยติดตามปริมาณการการใช้หน่วยความจำ สิ่งที่ถูกจัดเก็บในหน่วยความจำ และที่อยู่ในหน่วยความจำ
2. การจัดการ process พิจารณาว่ากระบวนการใดบ้างที่สามารถใช้หน่วยประมวลผลกลาง (CPU) ได้  ใช้งานเมื่อไหร่ และใช้นานเพียงใด
3. การจัดการไดรเวอร์ของอุปกรณ์ ทำหน้าที่เป็นสื่อกลาง/ล่ามระหว่างฮาร์ดแวร์และ process ต่างๆ
4. การจัดการคำสั่งเรียกใช้ระบบและความปลอดภัย รับคำขอบริการจาก process ต่างๆ

### ประเภทของ Kernel

1. Microkernel: เป็นสถาปัตยกรรมของระบบปฏิบัติการที่ kernel จะถูกทำให้มีขนาดเล็กที่สุดเท่าที่เป็นไปได้ โดยมีแค่ส่วนพื้นฐานที่จำเป็นต่อของระบบปฏิบัติการเท่านั้น

2. Monolithic kernel: เป็นสถาปัตยกรรมของระบบปฏิบัติการที่ทำในรูปแบบรวม ไดรเวอร์ของอุปกรณ์ ระบบไฟล์ และคำสั่งเรียกใช้ระบบมาในตัวของ Kernel เลย

3. Hybrid kernel: เป็นระบบปฏิบัติการที่รวมเอา Microkernel และ Monolithic kernel เข้าด้วยกัน เพื่อที่จะเอาข้อดีของทั้งสอง kernel มากลบข้อเสียซึ่งกันและกัน

4. Exokernel: เป็นสถาปัตยกรรมของระบบปฏิบัติการที่เน้นให้มี abstraction ในระบบให้น้อยที่สุด เสมือนเราไปควบคุมทรัพยากรของอุปกรณ์ต่างๆโดยตรง

5. Nanokernel: เป็นสถาปัตยกรรมของระบบปฏิบัติการที่ที่คล้ายกับ Microkernel แต่มีขนาดที่เล็กกว่าและทำให้มีประสิทธิภาพมากกว่าเมื่อเทียบกัน
