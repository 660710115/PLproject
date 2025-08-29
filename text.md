# Static Members
```Ruby
print "sun" #test
```
<details>
  <summary>Output</summary>

  This text is hidden until you click the dropdown.  
  You can use **Markdown formatting** here too.

  - Bullet list
  - **Bold text**
  - `Inline code`

</details>

หลายๆคนอาจจะเคยได้ยินคำว่า Static ในการเขียนโปรแกรมมาก่อน และอีกหลายๆคนอาจจะยังไม่เคยได้ยิน ก่อนอื่นเลยเรามาเริ่มทำความรู้จักกับคำว่า Static  เป็นสิ่งที่ใช้ได้กับตัวแปร และเมธอดของคลาส คุณสมบัติหลักๆขอStatic สามารถเข้าถึงได้ด้วยไม่ต้องสร้างobject สามารถเรียกใช้งานเมธอดผ่านคลาส ตัวแปรที่เป็น static จะผูกเข้ากับคลาสจะถูกแชร์ให้กับobject คลาสเดียวกัน ตัวอย่างเช่น กำหนดให้ class A เป็นคลาสที่มีตัวแปร static num มีค่าเป็น 0  จากนั้นเราสร้าง object b และ c ดังนั่น  b และcใช้ตัวแปร num ร่วมกัน