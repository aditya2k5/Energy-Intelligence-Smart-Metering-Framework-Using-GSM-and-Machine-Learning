# Energy Intelligence Smart Metering Framework Using GSM and Machine-Learning

# Why This Project 
With the escalation of energy demand and the prolif-
eration of power theft—especially in residential and institutional
settings intelligent energy management solutions have become
imperative. Conventional postpaid metering practices suffer from
inefficiencies related to manual readings, delayed anomaly detec-
tion, and a lack of real time monitoring or predictive analytics,
leading to operational losses and unreliable billing. This paper
proposes a smart prepaid energy metering solution that com-
bines Global System for Mobile Communication (GSM)-based
remote communication with machine learning-driven analytics to
provide integrated features, including prepaid billing, dynamic
tariff management, load forecasting, and theft detection, in a
unified and practical prototype. The system leverages Arduino or
Espressif Systems 32-bit (ESP32) microcontrollers and SIM800L
GSM modules for seamless, real-time monitoring and automated
SMS alerting. Three advanced machine learning models—Linear
Regression (LR), Support Vector Regression (SVR), and Random
Forest (RF)—were evaluated for short-term power consumption
prediction based on temporal and environmental data. Among
them, the Random Forest model achieved an R2 score of 0.98
and a mean absolute error of 741, indicating highly accurate
and reliable forecasts. Experimental assessments substantiate
the platform’s accuracy, operational scalability, and readiness
for real-world deployment, while highlighting future potential
through ongoing model refinement and the assimilation of larger
datasets.
# Functionality
## Prepaid Billing
The prepaid billing system uses a pulse sensor to detect electricity usage, deducting units from a stored balance in EEPROM. It displays the remaining units on an LCD and sends SMS alerts for low or zero balance. Power is disconnected automatically if the balance is zero, and recharging is done via GSM SMS commands. The system supports customizable tariff settings for flexible use.

## Power Theft Detection
The GSM-based prepaid energy meter detects power theft using sensors and updates the LCD with an alert. It sends SMS notifications with meter ID upon theft detection and resets automatically for further monitoring. The system also features ON/OFF control, enhancing security and real-time theft awareness.

## Tariff Calculation
The prepaid energy meter uses a real-time clock to apply different tariffs during peak (6–10 PM) and off-peak hours, charging higher rates when demand is high. This time-based pricing encourages efficient energy use, helps manage load, and stabilizes the grid by monitoring consumption and billing accordingly in real-time.

## Machine Learning
A robust machine learning framework was developed for
monthly electrical load forecasting using environmental and
temporal predictor.

The detailed development of this Machine Learning model - (https://github.com/aditya2k5/Forecasting-electric-load-using_ML.git)

# Schamtic Diagram 
<img width="648" height="367" alt="image" src="https://github.com/user-attachments/assets/323b5945-6205-4fd0-81e4-83fbf9ee69be" />

# Physical Hardware Circuit 
<img width="349" height="288" alt="image" src="https://github.com/user-attachments/assets/ac845d6c-41c3-439e-93a5-93987627ad69" />

