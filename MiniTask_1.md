Documentation of Mini-Task 1 -

Here are the 15 projects:

1. **Brainmotic**: 
This is an EEG brain-wave controlled smart home. It uses motor imagery using EEG electrodes to allow people to control various devices within their house like light switches, sockets, etc, through a smart device user interface. This is one of the slightly more difficult projects to replicate as research needs to be done regarding the analysis of these EEG signals. Link: https://hackaday.io/project/10600-brainmotic

2. **Biomonitor**: 
This is a device to measure mild electrical signals coming from the brain or from the heart. These signals need to be detected and then amplified, so both these aspects are taken care of in this project, before the signals are collected in the bluetooth module and dispatched. Link: https://hackaday.io/project/6760-biomonitor

3. **Landbeest walking robot**: This is an interesting walking mini-robot that can navigate terrain and walk within the house. It uses 2 servo motors, and a certain mechanical action that allows it to move. The motivation was to tackle the issues in robots with wheels which get stuck in certain places pretty often. Link: https://hackaday.io/project/165554-normal-air-conditioner-becomes-wifi-controlled

4. **Make air conditioner wifi-controlled**: 
In this project, we use an ESP8266 board which is positioned in a certain place to directly communicate with the AC through infrared. You can communicate with this controller using wifi on a smartphone app, and the AC is now effectively wifi-controlled. Not just that, additional features can be added (the controller can be made to detect room temperature/humidity and automatically adjust the AC). Link: https://hackaday.io/project/165554-normal-air-conditioner-becomes-wifi-controlled

5. **Belle**: This is a useful add-on that can be installed alongside doorbells in order to detect the event of the doorbell ringing by picking up signals directly from it, and then sending those signals through the IFTTT IoT interface to be able to notify you about it. https://hackaday.io/project/26347-belle-door-bell-alert-with-esp8266-ifttt

6. **Fall detector**: This project is pretty interesting, and essentially, it uses CV to determine whether a person has fallen or not. It is programmed using OpenCV and Python, using a Raspberry Pi module to run the software. There are a lot of different factors that need to be analysed while detecting a person's fall, such as the lack of movement, the place where the person isn't moving, and the sudden change in location of the centroid of the person's figure.  https://hackaday.io/project/12427-fall-detector

7. **Heart rate monitor**: This is a cool project, because it measures your heart rate and then displays it through a graph on a computer web app. It uses a MAX chip to measure heart rate and the samples are passed into the ESP32 controller. It's then passed through a band pass filter and the amplitude is measured with time which is displayed. https://hackaday.io/project/164155-esp-heart-rate-monitor

8. **Voice-controlled household lamps**: In this project, we create lamps that can be switched on and off through voice control. Essentially, the ESP32 microcontroller gets commands from an Amazon Echo device to toggle the lamp switch. The Amazon Echo device is paired up with the lamp, and it sends these commands whenever the Echo receives a particular voice command.  https://randomnerdtutorials.com/alexa-echo-with-esp32-and-esp8266/

9. **Air quality monitor**: A good low-cost air quality monitor can definitely be helpful in the household where rooms can get stuffy at times. It would be useful to have one of these providing real-time data regarding the temperature and relative humidity of the air in the room. This data can then be transmitted to a web server and be displayed. https://www.hackster.io/abid_hossain/air-quality-monitor-5f6afe

10. **TapLock**: It uses an accelerometer to detect a tap. The tapping pattern is then analysed by an ML model and matched with the 'password' pattern. This finally opens the lock. It seems like a feasible project that involves ML and detection through the accelerometer sensor. https://www.hackster.io/taplock/taplock-a-bike-lock-with-machine-learning-85641c

11. **Plant monitoring with IoT app**: This plant monitoring system can be useful in agriculture and in the household. Essentially, it measures data points on soil moisture, humidity, and temperature and updates it via an IoT app to the cloud real-time. Graphs can then be plotted on the app and analysed. https://www.hackster.io/magicbit0/esp32-plant-monitoring-with-arduino-iot-cloud-remote-app-fa4b75

12. **CAM pan and tilt web server**: This project uses two servo motors to rotate/move a camera along two axes. PWM signals are used to control the servo motors. Then we can couple this with a webpage and buttons on the page are used to remotely control the motors, thereby moving the camera. Whatever the camera captures is also displayed on the webpage. https://randomnerdtutorials.com/esp32-cam-pan-and-tilt-2-axis/

13. **OpenCV colour detection and tracking**: In this project, we create a web server which displays the video signals coming from a camera. Then, the software uses OpenCV to detect and look for a specific coloured object and track its centre of mass. https://randomnerdtutorials.com/esp32-cam-opencv-js-color-detection-tracking/

14. **DIY blood oxygen meter**: We can use the MAX oximeter sensor to directly detect blood oxygen levels. The data can then be fed to a mobile app and the app can display the value. https://www.instructables.com/DIY-Blood-Oxygen-Meter/

15. **Solar charging LiPo project**: This is a simple but interesting project that could be pretty useful to plot out the performance of a solar panel with change in weather conditions, time of the day, etc. It essentially calculates the voltage that the solar cell produces across the LiPo battery, and this data can be sent to a web server for plotting. https://hackaday.io/project/649-solar-charging-lipo-project
