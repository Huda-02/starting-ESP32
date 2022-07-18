# starting-ESP32
an algorithm to start the ESP32 board and make it blink. 
1.	وصل الجهاز باللوح عن طريق ال USB


2.	حمل Arduino IDE


3. عرف Arduino IDE على لوح ال ESP32


أ‌-	اذهب إلى: File>preferences>additional board manager URLs
وادخل الرابط الآتي : 
https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json  
ب‌-	اذهب إلى: tools>board>board manager
        واكتب ESP32 قم بتحميل الملف الظاهر  ESP32 by espressif systemsثم اغلق النافذة
 
4.	اختر اللوح الصحيح 
Tool>board اختر اللوح ESP32 Dev Modules
 
5.	انسخ الكود الآتي لل IDE

#define ONBOARD_LED  2

void setup() {
  pinMode(ONBOARD_LED,OUTPUT);
}

void loop() {
  delay(1000);
  digitalWrite(ONBOARD_LED,HIGH);
  delay(100);
  digitalWrite(ONBOARD_LED,LOW);
}

6.	حمل الكود لل  ESP32 
(اضغط على زر التحميل وهو السهم الأحمر في شريط الأدوات)
ملاحظة: في بعض النسخ قد يتطلب منك أن تضغط على زر التشغيل في اللوح نفسه لتحميل البرامج.
