# ESP32 with Servo motor

- note: we are using this website for simulation : https://wokwi.com/

## Step 1: click on ESP32 

<img width="959" alt="image" src="https://github.com/user-attachments/assets/d1c8bcdd-6e05-430b-8a25-ab4a328edc1a">

## Step 2: Click plus sign to get your Servo motor 
- you can add anything you want depending on your project

<img width="959" alt="image" src="https://github.com/user-attachments/assets/8af30e64-8e5e-4982-b462-f2fdf173908f">

## step 3: Start building the circuit & writing the code

![Screenshot 2024-07-23 091130](https://github.com/user-attachments/assets/fd518783-e999-4905-8ba8-9b69f75a31db)

```
#include<ESP32Servo.h>

Servo servo1;
int position=0;

void setup() {
  // put your setup code here, to run once:
  Serial.begin(115200);
  servo1.attach(4);
}

void loop() {
  // put your main code here, to run repeatedly:
  for(position=0; position<180;position++){
servo1.write(position);
delay(50);
  }
}
```

# note
you have to add the Servo library from (library manager) then add (ESP32Servo) 

<img width="959" alt="Screenshot 2024-07-23 091159" src="https://github.com/user-attachments/assets/52f04644-cc22-4e25-a01f-16c4b5c11407">

## finally
click on (Start Simulation) and Here we go, it works perfectly!


