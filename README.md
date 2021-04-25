# Thesis
โรงเพาะเห็ดอัจฉริยะโดยใช้เทคโนโลยีการสื่อสารไร้สายระยะไกล\
Smart Mushroom Farm using Long Range Wireless Communication Technology

บทคัดย่อ

ปริญญานิพนธ์นี้วัตถุประสงค์เพื่อออกแบบและสร้างโรงเพาะเห็ด ที่สามารถควบคุมสภาพแวดล้อมภายในโรงเรือนให้เหมาะสมต่อการออกดอกของเห็ดผ่านทางเว็บแอปพลิเคชันและวินโดว์แอปพลิเคชันเพื่อติดตามตรวจสอบและควบคุมระบบ และได้ประยุกต์ใช้งาน LoRa เพื่อเป็นตัวกลางการสื่อสารระหว่างโรงเรือนเพาะเห็ดและพื้นที่ที่มีสัญญาณอินเทอร์เน็ตเพื่อแก้ปัญหาสถานที่ตั้งของโรงเรือนที่อยู่ห่างไกลจากพื้นที่ครอบคลุมของสัญญาณอินเทอร์เน็ต

ระบบควบคุมสภาพแวดล้อมภายในโรงเรือนประกอบไปด้วยไมโครคอนโทรลเลอร์ (ESP32LoRa) ซึ่งเป็นตัวควบคุมระบบทั้งหมด โดยใช้เซนเซอร์ AM2315 วัดอุณหภูมิและความชื้นBH1750FVI วัดความสว่าง โดยมีอุปกรณ์ที่ใช้ในการควบคุมสภาพแวดล้อม เช่น พัดลม ปั๊ม หลอดไฟ และได้ประยุกต์ใช้งานตัวต้านทานตรวจสอบกระแส (Current Sense Resistors) เพื่อตรวจสอบสถานะการทำงานของอุปกรณ์ ส่วนของเว็บแอปพลิเคชันใช้ไมโครคอนโทรลเลอร์ (ESP32LoRa) เป็น Web Server และใช้แอปพลิเคชัน ngrok ที่ติดไว้บน Raspberry Pi ทำ Port forwarding เพื่อให้สามารถใช้งานเว็บแอปพลิเคชันได้จากทุกที่ที่สามารถเข้าถึงอินเทอร์เน็ต ส่วนของวินโดว์แอปพลิเคชันสามารถติดตามตรวจสอบและควบคุมโรงเรือนผ่านท่าง Serial Port ระหว่าง ไมโครคอนโทรลเลอร์และคอมพิวเตอร์

สรุปผลการดำเนินงาน การทดลองการทำงานของระบบสามารถทำงานได้ดี การทดลองเพาะเห็ดใช้เห็ดนางฟ้าในการทำการทดลองทั้งหมด 14 วันสามารถสรุปผลการทดลองได้ดังนี้ โรงเรือนที่ควบคุมสภาพแวดล้อม มีความกว้างของดอกเฉลี่ยเท่ากับ 7.66 เซนติเมตร มีน้ำหนักทั้งหมดเท่ากับ 1.06 กิโลกรัม โรงเรือนที่ไม่มีการควบคุมสภาพแวดล้อมมีความกว้างของดอกเฉลี่ยเท่ากับ 6.45 เซนติเมตร มีน้ำหนักทั้งหมดเท่ากับ 0.6 กิโลกรัม

Abstract

This thesis aims to design and construct a mushroom farm. That can control the environment in the farm to optimize the flowering of mushrooms through a web application and a window application to monitor and control the system. LoRa has been applied to serve as a communication medium between the mushroom house and the Internet-facing area to solve the problem of the location of the houses far from the Internet coverage area.

The farm environment control system consists of a microcontroller (ESP32LoRa) which controls the entire system. Using a sensor AM2315 to measure temperature and humidity, BH1750FVI measure the brightness. It has environment control devices such as fans, pumps, light bulbs, and has applied Current Sense Resistors to monitor the operating status of the device. The web application part uses a microcontroller (ESP32LoRa) as a web server and uses ngrok application installed on the Raspberry Pi to do port forwarding to be able to use the web application from anywhere that has access to the Internet. The window application can monitor and control the mushroom farm through the Serial Port between the microcontroller and the computer.

Conclusion of the experimental results the working of the system can work well. The mushroom cultivation experiments used grey oyster mushrooms for a total of 14 days the results of the experiment can be summarized as follows environment control farm has average flower width was 7.66 cm and the total weight was 1.06 kg. The farm without environment control has average flower width of 6.45 cm with a total weight of 0.6 kg. 
