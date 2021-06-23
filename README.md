# first-task-third-step
التحكم بالمحركات عن طريق مقاومة متغيرة 
اضيفت مقاومة متغيرة للدائرة السابقة وبرمجة الاردوينو لجعل المقاومة تتحكم بحركة المحرك في مجال 90 درجة 
كود الأردوينو:
#include <Servo.h>
Servo servo1;
Servo servo2;
Servo servo3;
Servo servo4;
Servo servo5;
int b=0;


void setup() 
{
  servo1.attach(1);
  servo2.attach(2);
  servo3.attach(3);
  servo4.attach(8);
  servo5.attach(10);

}
  
void loop() {
  b=analogRead(A1);
  b=map(b,0,1023,0,90);
  servo1.write(b);
  servo2.write(b);
  servo3.write(b);
  servo4.write(b);
  servo5.write(b);
                      
  }
  
  رابط مباشر من التينكركاد للمهمة :
  https://www.tinkercad.com/things/do7YTV4ZmU3-daring-turing-kup/editel?sharecode=hJ7dppkB0Q5Kb4jeSfsYiW2vmDV_zuJ2qaonklV9jrM
