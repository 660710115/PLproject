# Static Members

 หลายๆคนอาจจะเคยได้ยินคำว่า Static ในการเขียนโปรแกรมมาก่อน และอีกหลายๆคนอาจจะยังไม่เคยได้ยิน ก่อนอื่นเลยเรามาเริ่มทำความรู้จักกับคำว่า Static  เป็นสิ่งที่ใช้ได้กับตัวแปร และเมธอดของคลาส คุณสมบัติหลักๆขอStatic สามารถเข้าถึงได้ด้วยไม่ต้องสร้างobject สามารถเรียกใช้งานเมธอดผ่านคลาส ตัวแปรที่เป็น static จะผูกเข้ากับคลาสจะถูกแชร์ให้กับobject คลาสเดียวกัน ตัวอย่างเช่น 
 
 >กำหนดให้ class A เป็นคลาสที่มีตัวแปร static num มีค่าเป็น 0  จากนั้นเราสร้าง object b และ c ดังนั่น  b และcใช้ตัวแปร num ร่วมกัน




static ในแต่ละภาษาก็จะมีความแตกต่างกัน เช่นในภาษา C กับjava จะมี keywordในการบอกว่าเป็นstatic โดยใช้ “static” นำหน้าชื่อเมธอดหรือชื่อตัวแปร 
แต่ในภาษา Python และ Ruby ไม่มี keyword 
เราจะเรียนรู้เกี่ยวกับ static member ในภาษา Ruby กันซึ่ง static member จะมี 2 แบบ คือ

```Ruby
class A
  @@num = 0   # ตัวแปร class variable เริ่มต้นที่ 0

  def get
    @@num      # คืนค่าของ @@num
  end

  def set
    @@num = @@num + 1   # เพิ่มค่า @@num ทีละ 1
  end
end

c = A.new   # สร้าง instance c
b = A.new   # สร้าง instance b

b.set       # เรียก b.set → @@num = 0 + 1 = 1
puts "c value: #{c.get}"
puts "b value: #{b.get}"
```
<details>
  <summary>Output</summary>

  > c value: 1  
  > b value: 1  

</details>

> c value: 1  
> b value: 1 SEPARATE LINE

