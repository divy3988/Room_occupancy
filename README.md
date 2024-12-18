# Room_occupancy
Room Occupancy Monitoring System tracks room entry/exit using ultrasonic sensors, ESP32, and a seven-segment display. It updates real-time occupancy and sends WhatsApp alerts via CallMeBot when limits are exceeded. Includes code, flowchart, and setup instructions for easy implementation in managing room capacity efficiently.
Room Occupancy Monitoring System

Overview

This project tracks the number of people entering and leaving a room using ultrasonic sensors, an ESP32 microcontroller, and a seven-segment display. When the occupancy exceeds a specified limit, the system sends a WhatsApp alert using the CallMeBot API. The project is designed for spaces requiring real-time capacity management, such as offices, classrooms, or event venues.

Features

Real-time counting of people entering and leaving a room.

Display of the current occupancy count on a seven-segment display.

Automated WhatsApp alerts when the occupancy exceeds a predefined threshold.

Easy setup with detailed connection diagrams and step-by-step instructions.

Components Required

ESP32 Microcontroller

Ultrasonic Sensors (SRC04 or equivalent)

Seven-Segment Display (Common Anode)

Additional components: Breadboard, Jumper wires, Power supply

How It Works

Ultrasonic Sensors detect motion at the entry and exit points.

ESP32 processes the sensor data and determines the sequence of events to increment or decrement the count.

Seven-Segment Display shows the current number of people in the room.

When the count exceeds a specified limit, a WhatsApp alert is triggered using the CallMeBot API.

Setup Instructions

1. Hardware Setup

Connect the ultrasonic sensors to the ESP32 according to the provided connection diagram.

Wire the seven-segment display to the ESP32.

Power the system using a suitable power source.

2. Software Setup

Install the Arduino IDE and add the ESP32 board manager.

Include the required libraries (WiFi.h, HTTPClient.h, and UrlEncode.h).

Configure the WiFi credentials and CallMeBot API key in the code.

3. Deployment

Upload the code to the ESP32.

Power up the system and verify the setup.

WhatsApp Alert Setup

Save the CallMeBot contact number (+34 644 51 95 23) on your phone.

Send the message: I allow callmebot to send me messages.

Receive the API key via WhatsApp and configure it in the code.

Code Overview

Measure Distance: Calculates the distance using ultrasonic sensors to detect motion.

Update Count: Tracks entry/exit sequences to update the room occupancy count.

Display Count: Displays the count on the seven-segment display.

Send Alerts: Sends a WhatsApp alert if the occupancy exceeds the set limit.

Flowchart

Refer to the provided flowchart for a detailed explanation of the system logic.

Applications

Office spaces

Classrooms

Event venues

Any location requiring real-time capacity monitoring

References

Electronics Hub

Random Nerd Tutorials

CallMeBot API Documentation

License

This project is open-source and available under the MIT License. Feel free to modify and use it as needed.

Contribution

Contributions are welcome! Feel free to submit issues or pull requests for improvements or additional features.
