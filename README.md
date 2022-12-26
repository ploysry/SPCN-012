# SPCN-012


Hypervisor Technology
คือการจำลอง ฮาร์ดแวร์คอมพิวเตอร์ ซอฟต์แวร์ หรือเฟิร์มแวร์ที่สร้างเครื่องเสมือนที่มีการจัดการ การจัดสรรทรัพยากรแล้ว โดยเครื่องเสมือนแต่ละเครื่องสามารถเรียกใช้และระบบปฏิการในตัวมันเองได้ โดย โฮสต์ ใช้เรียกเครื่องสำหรับคอมพิวเตอร์ที่ติดตั้ง Hypervisor ส่วนที่เราสร้างเป็นเครื่องเสมือน
Hypervisor ทำหน้าที่เป็นตัวกลางระหว่างเครื่องโฮสต์และเครื่องเสมือน ทำหน้าที่ประสานการเข้าถึงสภาพแวดล้อมทางกายภาพให้เครื่องเสมือนหลายเครื่องสามารถเข้าถึงทรัพยากรร่วมกันได้ ทำให้ระบบปฏิบัติการหลายระบบสามารถทำงานพร้อมกันบน โฮสต์ ได้ และตั้งค่าระบบไม่ให้เกิดการทำงานที่ทับซ้อนหรือรบกวนกัน
cr.https://en.m.wikipedia.org/wiki/Hypervisor?fbclid=IwAR2RZca4rPfQHDsrzVhOMwQt5xqCo6OmnKdXMJwU4J8KEvX0aoiHBvTtr_Y

Contianer Technology
Containerสร้างขึ้นมาเพื่อแก้ปัญหาข้างต้น โดยมีฮาร์ดแวร์และ OS เพียงชุดเดียวกัน ลดความซ้ำซ้อนของการใช้ทรัพยากรลง ส่วนตัวแอพพลิเคชันและซอฟต์แวร์ซึ่งเป็นจุดที่แตกต่างกันไปก็จะมี "container" (เทียบได้กับ VM) มาครอบเพื่อแบ่งส่วนทรัพยากรไว้ไม่ให้ยุ่งกัน จุดเด่นของคอนเทนเนอร์จึงเป็นเรื่องการใช้ทรัพยากรที่น้อยกว่า virtualization มาก อิมเมจของคอนเทนเนอร์อาจมีขนาดเพียงกี่ไม่กี่สิบ MB ในขณะที่อิมเมจของ VM ต้องใช้พื้นที่ระดับหลาย GB นอกจากนี้ ระยะเวลาที่ใช้บูต, พลังซีพียูและปริมาณแรมที่ต้องใช้ ก็ลดลงตามไปด้วย
cr.https://www.blognone.com/node/105928?fbclid=IwAR125DKwxYHb8surmoSX0AN0iptX7krhxkREwKbyBOov9sD-birgq1wCqRQ


Monolithic Architecture
คือ สถาปัตยกรรมการออกแบบ และพัฒนาซอฟต์แวร์ ระบบหรือบริการ (Service) ที่รวมทุกส่วนเอาไว้ในสภาพแวดล้อม (Environment) เดียวกัน ใช้ฐานข้อมูลเดียวกัน (Database)
cr.https://ooneunhye.medium.com/monolithic-architecture-%E0%B8%84%E0%B8%B7%E0%B8%AD-%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3%E0%B9%80%E0%B8%AB%E0%B8%A3%E0%B8%AD-5737857fe9be


Proxmox VE ( proxmox virtual environment )
เป็นแพลตฟอร์มโอเพนซอร์สที่สมบูรณ์แบบสำหรับระบบเสมือนจริงแบบรวมทุกอย่างที่ผนวกรวม KVM hypervisor และ LXC คอนเทนเนอร์ระบบจัดเก็บข้อมูลและฟังก์ชันการทำงานของระบบเครือข่ายบนแพลตฟอร์มเดียวและสามารถจัดการกลุ่มการเข้าถึงข้อมูลที่มีประสิทธิภาพสูง และเครื่องมือการกู้คืนระบบได้โดยง่ายด้วย built- ในส่วนติดต่อการจัดการเว็บ
cr.https://www.bestinternet.co.th/single_blog.php?id=96&proxmox%20virtual%20environment%20%E0%B8%AB%E0%B8%A3%E0%B8%B7%E0%B8%AD%20proxmox%20ve%20(pve)%20%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3&fbclid=IwAR2CNlvvh1jFQeofXfkwzH9b3h1oqLe0969ragjFPv8WRmfUAEMDzgqWozk


Ceph 
เป็นระบบistributed storage แบบหนึ่ง หรือพูดง่ายๆ คือ เป็น storage ที่ทำงานบน cluster ของ computer node โดยในระบบ Ceph Storage ประกอบไปด้วย node 3 ประเภท คือ Monitor ทำหน้าที่ดูแลสถานะของ cluster. OSD (Object Storage Device) ทำหน้าที่อ่าน/เขียนข้อมูลตามคำสั่งของผู้ใช้
cr.https://www.throughwave.co.th/2017/04/10/%E0%B9%81%E0%B8%99%E0%B8%B0%E0%B8%99%E0%B8%B3-ceph-storage-distributed-storage-%E0%B8%A3%E0%B8%B9%E0%B8%9B%E0%B9%81%E0%B8%9A%E0%B8%9A%E0%B9%83%E0%B8%AB%E0%B8%A1%E0%B9%88%E0%B8%97%E0%B8%B5%E0%B9%88/?fbclid=IwAR1rs7sd9vM_E--fk24bEufc48u6Nk8Mhb7HURoeyVXmSSVhELQRFYxA8Ek#:~:text=Ceph%20Storage%20%E0%B9%80%E0%B8%9B%E0%B9%87%E0%B8%99%E0%B8%A3%E0%B8%B0%E0%B8%9A%E0%B8%9A%20distributed,%E0%B8%84%E0%B8%B3%E0%B8%AA%E0%B8%B1%E0%B9%88%E0%B8%87%E0%B8%82%E0%B8%AD%E0%B8%87%E0%B8%9C%E0%B8%B9%E0%B9%89%E0%B9%83%E0%B8%8A%E0%B9%89


NFS 
ย่อมาจาก Network File System เป็นตัวช่วยให้สามารถแชร์ข้อมูลผ่านLocal Networkได้ ถูกใช้งานเมื่อ ค.ศ.1984 แต่ยังมีการใช้กันอย่างแพร์หลายถึงปัจจุบัน NFS ใช้รูปแบบโครงสร้างที่เป็น Server และ Client ในการทำให้คอมพิวเตอร์หลาย ๆ เครื่องใน Local Network เดียวกันสามารถเข้าถึงไฟล์ได้ โดยฝั่งของ Server จะทำการตั้งค่า Folder ว่า Folder ไหนจะทำการแชร์ผ่าน Network ฝั่งของ Client ก็จะต้อง Mount ไฟล์ผ่าน Network โดยใช้คำสั่ง Mount ในอดีต NFS เป็นที่นิยมใช้งานกันบน Unix และ Linux เนื่องจาก NFS ถูกพัฒนาโดย Sun Microsystems ซึ่งเป็นบริษัทที่เป็น Vendor ของ Unix ปัจจุบัน NFS Protocol ได้กลายเป็น Standard Protocol ที่ง่ายต่อการใช้งานและในปัจจุบันสามารถที่จะใช้งานกับ Windows ได้
cr.https://blog.cloudhm.co.th/nfs-vs-smb/?fbclid=IwAR3cyb-jkur0BkrqpgI1Ax1yARyzwegZrGhLovXm7sJjgrCXGNxggPmLHb0
