## Debugging tutorial for TapLock

**Troubleshooting**

If there are issues, we'll need to properly identify the source of it.
There are multiple components working together in this prototype:
- ESP32 microcontroller
- Accelerometer
- Bluetooth
- The ML code to identify the pattern

If the lock is not opening, and no response is apparent, then we need to identify the source of the problem, which can be from any of the above components.

1. Check that all the components are working fine. The microcontroller should be running properly. Run a simple program to make the microcontroller to blink appropriately when an LED is attached. Copy/paste this code to do so:

```
int counter;

void setup()
{
  pinMode(13, OUTPUT);
}

void loop()
{
  for (counter = 0; counter < 10; ++counter) {
    digitalWrite(13, HIGH);
    delay(1000); // Wait for 1000 millisecond(s)
    digitalWrite(13, LOW);
    delay(1000); // Wait for 1000 millisecond(s)
  }
}
```

2. Then check that the accelerometer is working fine, by connecting it to the microcontroller and picking data from it onto the console. 
3. Also, ensure that the bluetooth module is working fine. Run this code:

```
char Incoming_value = 0;                //Variable for storing Incoming_value
void setup() 
{
  Serial.begin(9600);         //Sets the data rate in bits per second (baud) for serial data transmission
}
void loop()
{
  if(Serial.available() > 0)  
  {
    Incoming_value = Serial.read();      //Read the incoming data and store it into variable Incoming_value
    Serial.print(Incoming_value);        //Print Value of Incoming_value in Serial monitor
    Serial.print("\n");        //New line 
  }                            
} 
```
And try to send data through the module to the system and check that the appropriate information is visible on the Serial monitor.

4. Now we need to check if everything is working in our specific project. First connect the microcontroller directly to the computer and try to log the tap data to the serial monitor directly, by putting the exact time in milliseconds at which the tap occurred. Make sure this is workign properly.
5. Next, connect it to the bluetooth module and ensure that the data is being sent to the computer in the same way and being displayed on the serial monitor. If it still works, move to the next step.
6. Now, try to feed some test data into the ML model and make sure it recognises the data properly. Also, feed some of the data that you got in steps 4 and 5. If it still works, move on.
7. Considering that the above steps worked, there shouldn't be a problem. Try to integrate all the parts. If there is a problem at any step, then you have now identified the cause of the issue.


**Correction**

Once the issue is located, it should be fixed. If any part is malfunctioning, it should be replaced. If the parts are working fine, there might be some issue with the code, which should be fixed.

## Debugging tutorial for Voice-controlled lamps

**Troubleshooting**

1. Check that the microcontroller is working fine (follow the same steps as in the above tutorial).
2. First, check that the voice-recognition unit is working fine. Try to say commands and log the text onto the serial monitor, just to confirm this.
3. Then, check that the lamps are working. Make sure that they have battery, and also, ensure that when you hard-code the command to switch the lamp on and send it to the lamp through the microcontroller, it responds appropriately.
4. Finally, connect the voice-recognition unit and simultaneously monitor the output to the serial monitor, as well as the response of the lamp. 

**Correction**

Again, fix the issue once it is located. There may be some issue with the code, or with the device used. 

