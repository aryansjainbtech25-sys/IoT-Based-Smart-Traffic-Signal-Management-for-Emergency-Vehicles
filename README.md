# IoT-Based Smart Traffic Signal Management for Emergency Vehicles

## Problem

Current traffic signals operate on fixed timers or manual switches. They do not detect whether an approaching lane contains an emergency vehicle like an ambulance or fire truck.

Even when emergency vehicles are legally allowed to bypass red lights, they often get delayed because vehicles ahead have no time or space to move aside. In emergencies with multiple ambulances approaching the same intersection from different directions, their paths can cross and cause confusion, making traffic worse instead of better.

Additionally, ordinary citizens in urgent need—such as someone rushing a patient to the hospital in a private car—have no way to request priority at traffic signals. These delays can lead to serious consequences, including loss of life.

There is a clear need for a simple, low-cost system that can automatically detect emergency vehicles and clear their path through intersections.

## Proposed Solution

Our solution uses an Infrared (IR) sensor placed at each traffic signal to detect emergency vehicles.

How it works:

- Emergency vehicle identification: Each emergency vehicle (ambulance, fire truck, etc.) will carry a small IR emitter that sends a unique signal.

- Detection: When the vehicle approaches a traffic signal, the IR receiver at the junction detects this signal.

- Communication: The detection event is sent to a central dashboard/server over the Internet (using Wi-Fi/4G).

- Action: The server sends a command to the traffic signal controller to turn the light green for the lane where the emergency vehicle is detected.

- Clearing the path: The system also turns other lanes red to stop regular traffic, allowing the emergency vehicle to pass safely and quickly.

This system is low-cost, simple to deploy, and works in real-time to reduce emergency response delays.

## Objectives

## Hardware

## Software

## System Architecture

## Team Members

## Progress

## Future Work

After completing the core IR-based prototype, we plan to add the following enhancements:

- Camera-based detection: Use a camera and basic computer vision (OpenCV) to visually confirm the emergency vehicle (by detecting red/blue strobe lights). This will act as a backup verification method and reduce false detections.

- Manual SOS request: Provide a web-based dashboard or mobile app where drivers, patients, or bystanders can manually send an SOS signal to the server. This will help private vehicles carrying critical patients get priority even without an IR emitter.

- Live GPS tracking: Install GPS modules on emergency vehicles to track their real-time location. The server can then preemptively turn signals green as the vehicle approaches multiple intersections, creating a "green corridor" all the way to the destination. The system will also coordinate between multiple emergency vehicles to avoid path conflicts at the same junction.

These upgrades will transform our prototype into a complete, intelligent traffic management system.
