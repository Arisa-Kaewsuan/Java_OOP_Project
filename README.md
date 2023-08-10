# Object &nbsp;Oreinted &nbsp;with &nbsp;Java

### Exercise
  -  &nbsp;[จงออกแบบระบบห้องสมุดแบบ OOP พร้อมทั้งเขียน Data Flow Diagram ด้วยภาษา java]()
  -  &nbsp;[จงออกแบบระบบ E-commerce แบบ OOP พร้อมทั้งเขียน Data Flow Diagram ด้วยภาษา java]()

<br/><br/>

## 🤔 [Object &nbsp;Oreinted &nbsp;Principle](http://programmingbright.com/blog/?page=3)
:  &nbsp;&nbsp; concept ของ OOP ว่าคืออะไร  ดียังไง ทำไมควรฝึก  คำศัพท์เกี่ยวกับ OOP ที่ควรรู้จัก

<br/>

- &nbsp; ช่วยอธิบายหน่อยว่า [OOP](https://www.youtube.com/watch?v=OZH7TBoKyks&t=1739s) คืออะไร ประกอบไปด้วยอะไรบ้าง  แล้วมันดียังไง ?

      OOP คือ concept ที่มองทุกอย่างเป็น object (class) ออบเจ็บหนึ่งอย่างจะประกอบไปด้วย 2 ส่วน คือ
  
      1.  ลักษณะ (Atribute/property)/หน้าตา/UI (variables) : วิธีสังเกตุมักจะเป็น คำคุณศัพท์ / คำนาม เช่น สี, ขนาด
  
      2.  สิ่งที่มันทำได้/การกระทำ/Behavier (method) : วิธีสังเกตุมักจะเป็น คำกริยา เช่น move / bounce
  
    <br/>

            เมื่อเราสร้างมันเป็น object (class) แล้ว  มันจะสามารถใช้ คุณสมบัติ 4 อย่างได้ คือ encapsulation, abstraction,
      inheritance และ Polymorphism  คุณสมบัติทั้ง 4 อย่างนี้ช่วย ลดการเขียนซ้ำ ลดความซ้ำซ้อน เพราะเรา inherit มาแก้
      หรือเพิ่ม method ที่ต้องการเอาโดยไม่ต้องเขียนใหม่ เป็นการเอามาใช้ซ้ำ ช่วยประหยัดเวลาในการพัฒนา 
  
            การเขียนโค้ดแบบนี้ทำให้ได้  โค้ดที่อ่านง่ายเป็นระเบียบไม่รก เพราะ ไม่ต้องเขียนเรียงจากบนลงล่างเหมือนปกติ (เพราะคอมพิวเตอร์ประมวลผล
      ทีละบรรทัดแบบไล่บรรทัดจากบนลงล่าง เรียกว่า procedural หรือการทำงานแบบ sequence)  แต่เขียนแยกเป็น method/class แล้วเรียกใช้เอา
      มันจะไม่ทำงานถ้าเราไม่ได้เรียกใช้ การเขียนแยกแบบนี้คอมพิวเตอร์จะเริ่มทำจาก method main ก่อนเป็นอันดับแรก และไปทำ method อื่นๆตามที่ถูกเรียก
      ใช้ใน main การเขียนแยกแบบนี้ ยังทำให้ test และ แก้ไขง่ายด้วย  ทั้งยังเป็นมาตรฐานที่คนอื่นมาอ่านโค้ดเราก็จะเข้าใจได้ง่าย 
  
    <br/>
    
      วิธี หรือ ขั้นตอนการเขียนโปรแกรมแบบ OOP / การออกแบบโปรแกรมแบบ OOP (OOP Design)
  
      1.  ออกแบบว่าโปรแกรมของเราจะมี class อะไรบ้าง แต่ละคลาสทำอะไร รับข้อมูลอะไร วาดออกมาเป็น flowchart หรือ เขียนเป็น psudocode
  
      2.  แล้วมาสร้างเป็น class ใน class ประกอบไปด้วย
  
          -  constructor คือ " method ที่ชื่อเหมือนคลาส จะถูกเรียกใช้ครั้งเดียวตอน new class "  เป็นเหมือนการระบุลักษณะของคลาส
             # NOTE : ให้นึกภาพว่าการประกาศ constructor ของคลาส ก็เหมือนกับการที่ method รับ parameter มาใช้

          -  method ต่างๆ

  <br/>
  
- &nbsp; ช่วยอธิบายหน่อยว่า Encapsolution คืออะไร ?

            คือ การกำหนดการเข้าถึงด้วย modifier โดยจะประกาศ modifier ไว้หน้า class  method หรือ variables มีทั้งหมด 3 แบบ
  
      1.  public  :  class อื่น สามารถเรียกใช้ class  method หรือ variables ที่ระบุเป็น public นี้ได้
      
      2.  protected : class อื่น ไม่สามารถเรียกใช้ class  method หรือ variables นี้ได้ มีแค่ class เดียวกัน และ คลาสที่ inherit กัน
                      เท่านั้นที่ใช้ได้
                      # จะเห็นว่า protected กับ private ไม่สามารถใช้ประกาศหน้า class ได้
     
      3.  private : method และ variables ที่ระบุเป็น private จะใช้ได้แค่ภายในคลาสนี้
  <br/>
  
- &nbsp; ช่วยอธิบายหน่อยว่า  Inheritance คืออะไร ?

            คือ การ extend (สืบทอด) class มาใช้ทำให้สามารถใช้ทุกๆ method และ ทุกๆ variables ของ class นั้นได้โดยไม่ต้อง
      เขียนใหม่ ทำให้ลดการทำงานซ้ำ ช่วยประหยัดเวลาในการเขียนโปรแกรม  
  
            inheritance เปรียบเหมือนการที่ ลูกสืบทอด ลักษณะของพ่อแม่ แล้วยังสามารถทำอะไรที่พ่อแม่ทำไม่ได้อีกด้วย เราจึงเรียก
      -  class ที่ถูก extend สืบทอดคุณสมบัติ(method และ variables) ไปใช้ ว่า " superclass หรือ parentclass คือ คลาสแม่"
      -  และ class ที่ extend สืบทอดคุณสมบัติ(method และ variables) มาใช้ ว่า " subclass หรือ childclass คือ คลาสลูก"

  > ในภาษา java ใช้ syntax ```class [subclass] extends [superclass] { }``` เช่น ```class BoxWeight extends Box { }```
  <br/>
  
- &nbsp; Override  vs  Overloading คืออะไร เหมือนหรือต่างกันยังไง ?

      -  Overloading  คือ  method ที่ชื่อเหมือนกัน แต่ parameter ต่างกัน ทำงานเหมือนกัน แต่รับ parameter ต่างกัน
  
      -  Override  คือ  method ที่ชื่อ และ parameter เหมือนกัน แต่ทำงานต่างกัน เพราะ เรา override มันมาเขียนใหม่
  <br/>

- &nbsp; ช่วยอธิบายหน่อยว่า Abstraction คืออะไร ?

        L

  <br/>
  
- &nbsp; ช่วยอธิบายหน่อยว่า Polymorphism คืออะไร ?

        คือ การที่เราสืบทอดคลาสมา แล้วอยากเพิ่ม หรือ แก้ไข method จะทำได้ 2 แบบ คือ Override หรือ Overload

<br/><br/><br/>

## 👩‍💻 Object &nbsp;Oreinted &nbsp;Design
:  &nbsp;&nbsp; วิธีการออกแบบโปรแกรมแบบ OOP

  - Data Flow Diagram (DFD)
  - OOP Design
  - Context Diagram
  - UML
  - Class Diagram
 
              การออกแบบโปรแกรม  :  ในการจะสร้างโปรแกรมออกมาหนึ่งโปรแกรม ในการทำงานจริง จะมีขั้นตอนการวิเคราะห์ และออกแบบระบบ/โปรแกรม
        (System Analysis and Design) ซึ่งเป็นหน้าที่ของ Software Engineer ออกแบบแล้วส่งต่อให้ Programmer  ด้วย Data Processing
        Modeling ต่างๆ ซึ่งก็คือ Diagram ต่างๆ เราจึงต้องเรียนการวิเคราะห์
        ออกแบบ แล้วเขียนออกมาเป็น Diagram เพื่อที่ตอนทำงานจริงจะได้คุยงานกันได้เข้าใจ
 
        Data Processing Modeling หรือ Diagram ที่นิยมใช้กัน และควรรู้จักมีดังนี้
          -  Data Flow Diagram
          -  ER Diagram
 
        Tool ที่ใช้วาด Diagram สวยๆ และ ใช้งานสะดวก
          -  Visio
          -  Google Diagram
 
        DFD ประกอบด้วยสัญลักษณ์ดังนี้
          -  process
          -  External Entity
          -  Data Store

        Tool ที่ใช้วาด Diagram
