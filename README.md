# DYNAMIC-OTP-DRIVEN-SECURE-ACCESS-SYSTEM
## 📘 Overview
This embedded system uses GSM technology to control user access via OTP verification. Built with the LPC2148 microcontroller, it combines password authentication and RTC-based timing to ensure secure entry.

## 🎯 Objective
To develop a secure, time-limited OTP-based authentication system using embedded C and multiple hardware peripherals.

## 🔧 Hardware Components
LPC2148 Microcontroller

GSM Module (M660A)

16x2 LCD Display

4x4 Matrix Keypad

AT24C256 EEPROM

RTC Module

Switch (External Interrupt)

LED / Bulb / DC Motor

L293D Motor Driver

## 💻 Software Requirements
Embedded C Programming

KEIL µVision Compiler

Flash Magic Microcontroller Programming Tool

## ✨ Features
Password authentication via EEPROM

OTP generation and transmission via GSM

Real-time OTP validity enforcement with RTC

LCD interface for user guidance

Password reset through external interrupt

## 🔄 Workflow Summary
User enters password using keypad

If password is valid, system generates OTP

OTP is sent to user’s mobile via GSM

OTP timestamp saved using RTC

User enters OTP within the allowed time

Access granted if OTP is correct and timely

Access denied otherwise, system resets

Password can be updated using external interrupt

## 🧪 Testing Tips
Test each module separately: LCD, Keypad, UART, EEPROM, RTC

GSM module verified using AT commands through HyperTerminal

Ensure UART communication uses interrupt-driven logic

Integrate all modules into final application logic

## 📂 Repository Contents
Individual modules for peripherals

Central application file (main.c)

Configuration and utility headers
