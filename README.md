# AIR QUALITY INDEX
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
