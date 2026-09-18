# Week 2 - Using LEDs

## 1. Experiment Title

**Using LEDs**

---

## 2. Experiment Objectives

* Understand how to configure AVR ports.
* Understand how to set the input/output direction using `DDRA`.
* Control LED ON/OFF states using `PORTA`.
* Learn how to set port values using binary and hexadecimal numbers.

---

## 3. Experiment Theory

* `DDRA`: Sets the input/output direction of the PORTA pins.
* `PORTA`: Sets the output value of PORTA.
* Each LED can be controlled individually by using `0` and `1` for each bit.
* Binary values can be converted to hexadecimal values to make the code shorter and easier to read.

---

## 4. Experiment Procedure and Code

### Example 1

```c
#include <avr/io.h>

int main(){
    DDRA = 0b00000001;
    PORTA = 0b00000001;
}
```

In this example, the first bit of `DDRA` is set as an output, and the corresponding bit of `PORTA` is set to `1` to turn on the LED.

### Example 2

```c
#include <avr/io.h>

int main(){
    DDRA = 0b11111111;
    PORTA = 0b11111111;
}
```

### Example 3

```c
#include <avr/io.h>

int main(){
    DDRA = 0b11111111;
    PORTA = 0b00000001;
}
```

In Examples 2 and 3, all PORTA pins are configured as outputs, and different values are assigned to `PORTA` to compare the LED output states.

---

## 5. Hexadecimal Representation

Binary values can be converted into hexadecimal values to make the code more concise.

```c
#include <avr/io.h>

int main(){
    DDRA = 0xFF;
    PORTA = 0xFF;
}
```

The experiment also introduces the use of hexadecimal values such as `DDRA = 0xFF` and `PORTA = 0xFF`.

---

## 6. Experiment Results

* The LED-connected PORTA pins were configured as outputs using `DDRA`.
* The LED ON/OFF states could be controlled by changing the value of `PORTA`.
* Both binary and hexadecimal values could be used to control the LEDs.
* The experiment included turning on LD3, LD6, and LD8.

---

## 7. Discussion

In this experiment, I learned the basic method of controlling LEDs using the AVR GPIO port. I learned the difference between `DDRA` and `PORTA` and how each bit can be used to control individual LEDs.

I also learned how to represent port values using both binary and hexadecimal numbers. Using hexadecimal values makes the code more concise and easier to read.

The experiment also introduced a better coding practice. Instead of directly assigning a value to `PORTA`, it is recommended to declare a variable and assign the desired value to the variable first.

For example:

```c
PORTA = PortValue;
```

This approach makes the code more organized and easier to manage.
