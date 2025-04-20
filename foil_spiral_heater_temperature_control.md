# Temperature Control Design of a Foil Spiral Heater

**Author**: Ville Johannes Savolainen  
**Date**: April 19, 2025  
**Disclosure Type**: Public Prior Art 
---

The foil spiral heater is typically controlled using **PWM (Pulse Width Modulation)**. Temperature is estimated by observing the increasing resistance of the foil as it heats up — a property that changes predictably with temperature in materials like stainless steel. This resistance is monitored by the microcontroller, and temperature is calculated in software.

## Improving Accuracy

To increase control precision and allow for the use of different foil materials (including those with less significant temperature-resistance characteristics), additional temperature sensing techniques can be applied:

### 1. **Direct Temperature Sensors**
- **Thermocouples**
- **NTC thermistors**
- Other temperature sensing elements

These can provide direct readings of the heater or surrounding areas for more accurate feedback.

### 2. **Power-Based Temperature Estimation**
Temperature can be derived indirectly by evaluating:
- **Incoming air temperature**
- **Heater power consumption**
- **Airflow speed**

Airflow speed can be estimated using a **pressure sensor** that detects pressure drops caused by inhalation. With a microcontroller, this data can be processed in real-time to compute an accurate temperature estimate and enable dynamic adjustment of the heating power.

### 3. **Infrared (IR) Sensing**
An **IR temperature sensor** can be used to measure radiated heat from the foil. This allows for **non-contact temperature sensing**, which is particularly useful when direct measurements are impractical.

## Summary

By combining software-driven estimation and multiple sensing strategies, we can:
- Achieve more stable temperature regulation
- Improve responsiveness to changing airflow and ambient conditions
- Support the use of alternative foil materials beyond stainless steel

These methods allow for greater flexibility and precision in applications requiring consistent thermal output, such as inhalation-based systems or portable heating units.

## Intent

This disclosure is published to establish prior art and prevent exclusive patent claims on foil spiral heater temperature control systems. This includes methods involving resistance-based temperature estimation, power and airflow-based thermal modeling, and optional use of thermocouples, NTCs, or infrared sensors for improving accuracy and stability.
