#include <Servo.h>

Servo myservo3;
Servo myservo5;
Servo myservo6;
Servo myservo9;
Servo myservo10;
Servo myservo11;
Servo myservo12;


int pos = 0;    
void setup() {
  myservo3.attach(3);
  myservo5.attach(5);
  myservo6.attach(6);
  myservo9.attach(9);
  myservo10.attach(10);
  myservo11.attach(11);
  myservo12.attach(12);
} 

void pluck1(){
  myservo12.write(80);
  //if(myservo12.read()==80)myservo12.write(0);
  }

void pluck2(){
  myservo12.write(0);
  //if(myservo12.read()==80)myservo12.write(0);
  }

void press2(){
  myservo3.write(10);
  }

void release2(){
  myservo3.write(40);
}

void press3(){
  myservo5.write(10);
  }

void release3(){
  myservo5.write(40);
}

void press4(){
  myservo6.write(10);
  }

void release4(){
  myservo6.write(40);
}

void press5(){
  myservo9.write(10);
  }

void release5(){
  myservo9.write(40);
}

void press7(){
  myservo10.write(10);
  }

void release7(){
  myservo10.write(40);
}

void press9(){
  myservo11.write(20);
  }

void release9(){
  myservo11.write(40);
}







void loop() {

  myservo12.write(0);
  
  press2();
  pluck1();
  delay(500);
  release2();
  
  pluck2();
  delay(500);

  press2();
  pluck1();
  delay(500);
  release2();

  press3();
  pluck2();
  delay(500);
  release3();

  delay(500);

  press2();
  pluck1();
  delay(500);
  release2();
  
  pluck2();
  delay(500);

  press2();
  pluck1();
  delay(500);
  release2();

  press3();
  pluck2();
  delay(500);
  release3();

  delay(500);

  press2();
  pluck1();
  delay(500);
  release2();
  
  pluck2();
  delay(500);

  press2();
  pluck1();
  delay(500);
  release2();

  press3();
  pluck2();
  delay(500);
  release3();

  pluck1();
  delay(500);

  delay(500);
}
