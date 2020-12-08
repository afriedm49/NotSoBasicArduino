# NotSoBasicArduino
 The follwing files are my second foray into Arduino
 
 
## Table of Contents
* [Table of Contents](#TableOfContents)
* [LED_Fade](#LED_Fade)
* [ArduinoReview](#ArduinoReview)
* [HelloFunctions](#HelloFunctions)
* [NewPing](#NewPing) 

---

## LED_Fade

### Description & Code


Here's how you make code look like code:

```C++
  analogWrite(led, brightness);

  // change the brightness for next time through the loop:
  brightness = brightness + fadeAmount;

  // reverse the direction of the fading at the ends of the fade:
  if (brightness <= 0 || brightness >= 255) {
    fadeAmount = -fadeAmount;
  }
```

This is used to fade an led on and off. The Led will go from on to off slowly in a specific amount of time.
### Evidence
[LED Fade on Arduino Create](https://create.arduino.cc/editor/helmstk1/9e044cca-43d7-4d93-885f-e6dec5b4f769/preview)

### Images
Curcuit Fritzing from makerspaces.com:
<img src = "https://www.makerspaces.com/wp-content/uploads/2017/05/2-Blink-an-LED_LARGE.jpg" width = "300"> 
### Reflection
This helped me remember how to write basic code. In Engineering 1 last year, we made this exact code, but I didn't remember how to do it until now.

## ArduinoReview

### Description & Code




```C++
int delayVar = 1000;
int LED = 8;
void setup() {

  Serial.begin(9600);
  pinMode(LED, OUTPUT);
}

void loop() {

  if (delayVar > 100) {
    Serial.println(delayVar);
    digitalWrite(LED, HIGH);
    delay(delayVar);
    digitalWrite(LED, LOW);
    delay(delayVar);
    delayVar = delayVar - 100;
  }
  else {
   Serial.println(delayVar);
    digitalWrite(LED, HIGH);
    delay(delayVar);
    digitalWrite(LED, LOW);
    delay(delayVar);

  }
}
```
This code makes an LED blink for a shorter amount of time each time it blinks, starting at 1 second on and off, and then decreasing by 100 milliseconds each blink. A variable is used, starting at 1000, and lowering by 100 each loop, until it reaches 100.

### Evidence
[Arduino Review Assignment on Arduino Create](https://create.arduino.cc/editor/afriedm49/d85e6356-de43-4c6c-b82f-95ef524ca9bd)

### Images
Curcuit Fritzing from makerspaces.com:
<img src = "https://www.makerspaces.com/wp-content/uploads/2017/05/2-Blink-an-LED_LARGE.jpg" width = "300"> 
### Reflection
This assignment was useful for a different type of Variable than the "Variable LED blink": 
I used the variable to change the amount of time it would delay, instead of a counter for the number of times the loop went through.

## HelloFunctions

### Description & Code
Description goes here

Here's how you make code look like code:

```C++
Code goes here
```
Talk about how the code works, here....

### Evidence
link goes here

### Images
draw it yourself, take a picture, make a fritzing, whatever you want to EFFECTIVELY communicate how its put together.

### Reflection

## NewPing

### Description & Code
Description goes here

Here's how you make code look like code:

```C++
Code goes here
```
Talk about how the code works, here....

### Evidence
link goes here

### Images
draw it yourself, take a picture, make a fritzing, whatever you want to EFFECTIVELY communicate how its put together.

### Reflection

