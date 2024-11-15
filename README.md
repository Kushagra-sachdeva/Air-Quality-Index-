## AIR QUALITY INDEX
# Project Overview

This project aims to monitor the air quality by measuring various pollutants in the air using an Arduino-based system. The system will provide real-time data and display the Air Quality Index (AQI) for the environment, making it easier to assess the level of pollution and make necessary adjustments to ensure better air quality.

# Components Required

	•	Arduino Uno (or any compatible Arduino board)
	•	MQ-135 Gas Sensor (for detecting ammonia, carbon dioxide, alcohol, etc.)
	•	LCD Display (16x2 or similar)
	•	Jumper wires
	•	Breadboard
	•	5V Power Supply (or USB cable for Arduino)
	•	Resistors (for wiring purposes)
	•	Push button (optional) (for manual reset)

# Optional

	•	Buzzer or LED (to alert when AQI crosses a certain threshold)

# Features

	•	Real-time AQI Measurement: The system will calculate AQI based on the data from the MQ-135 sensor.
	•	LCD Display: Displays AQI and pollutant levels in real-time.
	•	Air Quality Classification: AQI values will be classified into various categories (e.g., Good, Moderate, Unhealthy, etc.).
	•	Alerts: Optional buzzer or LED indicator to alert when the air quality is unhealthy.

# Circuit Diagram


# Basic Connections:

	•	MQ-135 Sensor:
	•	VCC → 5V
	•	GND → GND
	•	A0 → Analog Pin A0 (or any available analog pin)
	•	LCD Display (16x2):
	•	VCC → 5V
	•	GND → GND
	•	SDA → A4 (on Arduino Uno)
	•	SCL → A5 (on Arduino Uno)

# If using a buzzer or LED for alerts:

	•	Buzzer/LED:
	•	Connect the positive leg to a digital pin (e.g., Pin 12)
	•	Connect the negative leg to GND

# Setup

	1.	Connect the Components:
	•	Connect the MQ-135 sensor to the analog input pin of the Arduino (e.g., A0).
	•	Connect the 16x2 LCD display to the appropriate SDA and SCL pins.
	•	If using an LED or buzzer, wire it to a digital pin for triggering when AQI crosses a threshold.
	2.	Upload Code to Arduino:
	•	Open the Arduino IDE and paste the following code (see below).
	•	Select the appropriate board and port in the Tools menu.
	•	Click the Upload button.
	3.	Power Up:
	•	Power up the Arduino using a USB cable or external power supply.
	•	The system will start measuring the air quality and display the results on the LCD.
# Explanation:

	•	MQ-135 Sensor: Measures the gas concentration in the air and sends the value to the Arduino board.
	•	Voltage to PPM: The sensor provides an analog output that corresponds to the concentration of pollutants, which is then converted to PPM (parts per million).
	•	LCD Display: Shows the AQI value and a classification of air quality (Good, Moderate, Unhealthy, etc.).

# How to Use

	1.	Run the System: Once the components are wired and the code is uploaded, the system will continuously monitor the air quality.
	2.	View AQI: The LCD will display the AQI along with a classification of the air quality based on the sensor data.
	3.	Alerts: If you have connected a buzzer or LED, it will trigger when the air quality becomes unhealthy or worse.

# Calibration

The MQ-135 sensor requires calibration for accurate measurements. The calibration process typically involves:

	•	Using known concentrations of gases (like CO2 or ammonia) and adjusting the sensor’s output values.
	•	Using a reference AQI chart and adjusting the formula used in the code to match real-world measurements.

For more accurate results, it is recommended to calibrate the sensor using specific gas sources or professional equipment.

# Troubleshooting

	•	LCD not displaying correctly: Check the wiring of the LCD and ensure it is properly connected to the correct SDA/SCL pins. Make sure the contrast is adjusted correctly.
	•	No data on the screen: Make sure the MQ-135 sensor is connected correctly to the analog input pin and that the sensor is working.
	•	AQI values are too high or too low: Adjust the formula in the code based on the sensor’s calibration and environmental conditions.

# Future Enhancements

	•	Web or Mobile Interface: Connect the Arduino to a server for remote monitoring via web or mobile app.
	•	Multiple Sensors: Integrate additional sensors to measure other air pollutants such as PM2.5, CO2, etc.
	•	Data Logging: Add a feature to log air quality data over time for analysis and reporting.
 
# Conclusion

This project provides a simple yet effective way to monitor air quality in real-time. Using Arduino and the MQ-135 sensor, it enables users to visualize and classify air quality based on live readings. This project is a great start for building IoT-based environmental monitoring systems.
