# Review-HW---simulation-CiscoPackettracer-




- التطبيق 

في هذا المشروع سيتم إنشاء دائره كهربائية وهم المواضيع هي : 

-  تحقيق المبادئ الرئيسية في الكهرباء ( قانون اوم - التأريض ). 
-  إنشاء دائرة كهربائية على الأدوينو.






 

تطبيق على المنصة الافتراضية 

راح نحتاج للتطبيق 
١- UNO 
٢-breadboard  


![](https://paper-attachments.dropbox.com/s_51D4B74E1E15B4A8DD2A824E39329518431ACBC50C4720496AE72BA41299FC5E_1640546651710_Screen+Shot+1443-05-22+at+10.23.00+PM.png)


لو لاحظنا هنا في حال وصلنا هنا GND عشان نكمل الدائرة الكهربائية راح يكون الخط الافقي جميعة يحمل نفس القيمة . 


![](https://paper-attachments.dropbox.com/s_51D4B74E1E15B4A8DD2A824E39329518431ACBC50C4720496AE72BA41299FC5E_1640590179379_Screen+Shot+1443-05-22+at+10.23.00+PM.png)


١- راح نوصل GND في breadboard و Power عرفا يستخدم السلك الاسود GRN و السلك الأحمر POWERوأيضا نوصل GRN (-) و POWER (+) في حال توصيلGND يكون كل الصف  GND وأيضا في حال POWER.

![](https://paper-attachments.dropbox.com/s_51D4B74E1E15B4A8DD2A824E39329518431ACBC50C4720496AE72BA41299FC5E_1640547264729_Screen+Shot+1443-05-22+at+10.32.28+PM.png)



هنا راح أحتاج اوصل PIN في الاردوينو نفسة  مثلا لو كان بنسوي Led (ضوء) راح يكون Digital وهو اللي بينقل التيار وهذا PIN اللي راح نكتب عليه CODE 

- Resistor ( يخفف التيار ).
![](https://paper-attachments.dropbox.com/s_51D4B74E1E15B4A8DD2A824E39329518431ACBC50C4720496AE72BA41299FC5E_1640592118964_150-ohm-resistor-TRUE-.png)


 

- LED  لو لاحظنا في واحد طويل وواحد قصير 


![](https://paper-attachments.dropbox.com/s_51D4B74E1E15B4A8DD2A824E39329518431ACBC50C4720496AE72BA41299FC5E_1640591747045_0EsSakdaVBAG8SRTc7uYASpCqCiZn8cjaQ5Sq4yo.jpeg)



![](https://paper-attachments.dropbox.com/s_51D4B74E1E15B4A8DD2A824E39329518431ACBC50C4720496AE72BA41299FC5E_1640597365810_images.png)



![](https://paper-attachments.dropbox.com/s_51D4B74E1E15B4A8DD2A824E39329518431ACBC50C4720496AE72BA41299FC5E_1640549212170_Screen+Shot+1443-05-22+at+11.06.23+PM.png)

الكود البرمجي 

بلغة C++
 
أول شي نعرف LED  ومن ثم زي مانشوف فية ميثود pinMode () نكتب فيها المتغيرات led,OUTPUT
وبعدها دخلت في loop اللي هي  عن delay هنا متى يكون low ومتى يكون high . 



    
    int led = 7; 
    
    void setup()
    {
      pinMode(led,OUTPUT );
    }
    
    void loop()
    {
      digitalWrite(led, HIGH);
      delay(1000); // Wait for 1000 millisecond(s)
      digitalWrite(led, LOW);
      delay(1000); // Wait for 1000 millisecond(s)
    }
----------
