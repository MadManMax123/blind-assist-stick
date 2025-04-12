**Smart Assist Stick for the Visually Impaired**

[![Netlify Status](https://api.netlify.com/api/v1/badges/6bdc86a4-725f-4978-b6d0-c9fbad948e1e/deploy-status)](https://app.netlify.com/sites/assistick/deploys)

**Objective:**
Develop a walking stick that detects nearby obstacles, identifies objects, and provides audio feedback using vibration motors and voice output, enhancing mobility and safety for visually impaired individuals.

**Core Features Overview:**
The smart assist stick integrates various advanced technologies to improve the mobility and safety of visually impaired individuals:

1. **Obstacle Detection:** Ultrasonic sensors measure distance and activate internal vibration motors. Vibration intensity increases as obstacles approach.
2. **Object Recognition:** A Pi Camera paired with MobileNet SSD identifies and classifies objects like humans, pets, and vehicles.
3. **Voice Feedback:** Recognized objects are announced through MP3s using an AUX-connected audio device.
4. **USB-C Charging:** Fast and reliable power input via USB-C, ensuring easy compatibility.
5. **LED Battery Indicator:** Five-segment LEDs indicate charge level and blink during charging.
6. **Internal Build:** Vibration motors are embedded in a hollow PVC stick, creating a sleek, wire-free design.
7. **Pattern-based Vibration:** Custom vibration signals indicate spatial and urgency-based context:
   - Fast Pulse – Danger close
   - Slow Pulse – Distant object
   - Left/Right Pulse – Directional cue
   - Continuous Buzz – Path blocked
8. **GPS Tracking:** Real-time location tracking assists caregivers and supports navigation.
9. **Emergency Button:** A distress signal is sent with GPS coordinates when the button is pressed, along with visual/audio alarms if necessary.
10. **Fingerprint Authentication:** Ensures only authorized users can access core and emergency features.
11. **Gyroscope & Fall Detection:** Detects falls and tilts, triggering emergency alerts to caregivers.
12. **Solar Charging:** Integrated solar charging capabilities provide additional power during operation.
13. **Weather Alerts:** Provides spoken warnings about adverse weather conditions.
14. **Step Tracking:** Monitors steps, distance, heart rate, and calories.

**User Manual:**
- **Powering On:** Charge via USB-C and hold the power button for 3 seconds to power on.
- **Fingerprint Unlock:** Scan your finger to unlock the system.
- **Fingerprint Registration:** Register new users by scanning the finger three times in setup mode.
- **Navigation Mode:** Begin walking. The stick vibrates based on proximity and direction.
- **Audio Mode:** Use earphones connected to the AUX jack for audio feedback on recognized objects.
- **Charging:** Connect the USB-C port to charge the device. LED bars indicate the charge status.
- **Emergency Use:** Hold the emergency button for 3 seconds to send alerts and share your GPS location.
- **Shutdown:** Hold the power button for 3 seconds to switch off.

**Workflow:**
1. **Obstacle Detection:** Use ultrasonic sensors to detect objects and trigger vibrations.
2. **Object Recognition:** Capture images with Pi Camera and identify objects using MobileNet SSD.
3. **Voice Output:** Play corresponding MP3 messages for identified objects.
4. **Emergency Function:** Trigger alerts when the emergency button is pressed.
5. **Fingerprint Access:** Authenticate users and restrict emergency and tracking access.
6. **Fall Detection:** Use gyroscope and accelerometer data to detect falls and send emergency alerts.
7. **Charging:** USB-C charging with LED indicators. Optionally use solar charging.
8. **GPS & Weather Alerts:** Track real-time location and provide weather alerts.
9. **Audio Mode:** Provide spoken feedback through the AUX jack.
10. **Step Tracking:** Monitor steps and health data, providing feedback and integration with health apps.

**Hardware Requirements:**
- Raspberry Pi 4
- Pi Camera Module v2
- Ultrasonic Sensors (HC-SR04) × 2-3
- Vibration Motors × 5–10
- Motor Driver (L298N or Transistors)
- Speaker/Earphones (AUX)
- LED Battery Indicators × 5
- USB-C Charging Module
- Li-ion Battery Pack or Power Bank
- GPS Module (NEO-6M)
- Emergency Button Switch
- Fingerprint Sensor Module (e.g., R307)
- Gyroscope + Accelerometer (e.g., MPU6050)
- PVC pipe (for the stick)

**Software Requirements:**
- Raspberry Pi OS (Lite)
- Python 3
- OpenCV
- TensorFlow Lite / MobileNet
- pygame or omxplayer
- GPSD (for GPS module)
- Adafruit Fingerprint Library
- MPU6050 Python Library
- Weather API integration (e.g., OpenWeatherMap API)

**Extended Features & Optional Upgrades:**
- AI-powered voice assistant for contextual feedback.
- Advanced fall detection with timed voice responses and auto-alerts.
- Mobile app integration to monitor battery, location, and emergency logs remotely.
- Real-time cloud dashboard for caregivers to track location and logs.
- Night navigation lights for low-light environments.
- Smart terrain classification using pressure and tilt sensors.
- Adjustable vibration intensity via an external app.
- Voice-controlled emergency contact dialing via smart assistants (e.g., Google Assistant, Siri).

**We Value Your Feedback:**
Satyaki Bandopadhyay  
Email: satyaki.b2009@gmail.com  
Designed by Satyaki Bandopadhyay  
Website development made with AI  
Form automation with Formspree.
