เพื่อรันโปรแกรม TSP ที่ใช้ Socket เพื่อเชื่อมต่อระหว่างเซิร์ฟเวอร์และโหนดใน Java โดยใช้คลาส TSPServer และ TSPClient ตามที่ได้แสดงไว้ข้างต้น คุณสามารถทำตามขั้นตอนดังต่อไปนี้:
#ต้องRun Client 3 เครื่อง แล้วRun Server 1 เครื่อง โดยต้องRun Serverก่อนเเล้วจึงRun Client เนื่องจากเราใช้Physical node
วิธีการรัน
1. เปิดโปรแกรม Integrated Development Environment (IDE) ที่คุณใช้ในการเขียนและรันโปรแกรม Java ได้เช่น IntelliJ IDEA, Eclipse, NetBeans, หรืออื่น ๆ

2. สร้างโปรเจกต์ใหม่และสร้างไฟล์ Java สำหรับคลาส TSPServer และ TSPClient ในโปรเจกต์ของคุณ

3. คัดลอกโค้ดสำหรับคลาส TSPServer และวางในไฟล์ TSPServer.java ในโปรเจกต์ของคุณ

4. คัดลอกโค้ดสำหรับคลาส TSPClient และวางในไฟล์ TSPClient.java ในโปรเจกต์ของคุณ

5. บันทึกและคอมไพล์โค้ด Java ในโปรเจกต์ของคุณ

6. เปิดเทอร์มินัลหรือหน้าต่างที่ให้คุณป้อนคำสั่งในระบบปฏิบัติการของคุณ

7. เข้าสู่ไดเรกทอรีของโปรเจกต์ Java ของคุณที่มีไฟล์ TSPServer.java และ TSPClient.java

8. รันคำสั่ง javac TSPServer.java เพื่อคอมไพล์ไฟล์ TSPServer.java

9. รันคำสั่ง javac TSPClient.java เพื่อคอมไพล์ไฟล์ TSPClient.java

10. หลังจากคอมไพล์สำเร็จโปรแกรม TSP จะถูกคอมไพล์เป็นไฟล์ bytecode (.class)

11. ในเทอร์มินัลหรือหน้าต่างคอมพิ

วเตอร์ที่แยกออกมาใหม่, รันคำสั่ง java TSPServer เพื่อเริ่มเซิร์ฟเวอร์ TSP

12. เปิดหน้าต่างที่แยกออกมาใหม่อีกหนึ่งเทอร์มินัลหรือหน้าต่างคอมพิวเตอร์, รันคำสั่ง java TSPClient เพื่อเริ่มโหนด TSP

13. โหนดจะเชื่อมต่อกับเซิร์ฟเวอร์ TSP และส่งข้อมูลโหนดไปยังเซิร์ฟเวอร์ โดยเซิร์ฟเวอร์จะประมวลผลและส่งคำตอบกลับมาที่โหนด

14. ผลลัพธ์จะปรากฏในทั้งเซิร์ฟเวอร์และโหนด TSP

โปรแกรม TSP ที่ใช้ Socket ในการเชื่อมต่อระหว่างเซิร์ฟเวอร์และโหนดจะเปิดพอร์ตที่ 12345 สำหรับการเชื่อมต่อ หากคุณต้องการเปลี่ยนพอร์ต คุณสามารถแก้ไขค่าคงที่ PORT ในคลาส TSPServer และ SERVER_PORT ในคลาส TSPClient เป็นพอร์ตที่คุณต้องการใช้งาน
