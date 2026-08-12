# STM32 I2C LCD Interfacing

An STM32-based project demonstrating **16×2 I2C LCD interfacing** using the **STM32 NUCLEO-F401RE** development board.

The project uses the STM32 I2C peripheral to communicate with the LCD through an I2C interface, reducing the number of GPIO pins required for LCD communication.

---

## 📌 Project Overview

This project demonstrates how to interface a **16×2 LCD with an I2C module** using the STM32 NUCLEO-F401RE board.

The LCD is controlled through the STM32's I2C peripheral, while a custom LCD driver is implemented using separate `lcd.c` and `lcd.h` files.

The project was developed using **STM32CubeIDE** and **STM32CubeMX configuration**.

---

## 🔧 Hardware Used

- STM32 NUCLEO-F401RE
- 16×2 LCD Display
- I2C LCD Module
- Jumper Wires
- Breadboard

---
## Circuit Diagram

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/a1007aa9-2833-476a-8e31-b7c3de4e0913" />


## ⚙️ Software & Tools

- STM32CubeIDE
- STM32CubeMX
- Embedded C
- HAL Library
- I2C Communication

---

## 🔌 Communication

The LCD communicates with the STM32 through the **I2C protocol**.

### I2C Interface

| Signal | STM32 |
|---|---|
| SDA | I2C SDA |
| SCL | I2C SCL |
| VCC | 5V |
| GND | GND |

The exact pin configuration is available in the `.ioc` configuration file included in this repository.

---

## 🧩 Project Structure

```text
STM32-I2C-LCD/
│
├── Core/
│   ├── Inc/
│   │   └── lcd.h
│   │
│   └── Src/
│       ├── lcd.c
│       └── main.c
│
├── README.md
│
└── llcc_i2c.ioc
