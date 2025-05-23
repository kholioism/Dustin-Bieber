# 🧹 Autonomous Vacuum Cleaner (STM32F103C8T6 + RTOS)

This project is an RTOS-based autonomous vacuum cleaner built on the STM32F103C8T6 microcontroller. It uses ultrasonic sensors and bumper switches for obstacle detection and avoidance, with FreeRTOS managing the system's concurrent tasks.

## 🚀 Features

- Real-time obstacle avoidance using ultrasonic sensors (HC-SR04)
- Collision detection via bumper switches
- DC motor control using PWM via L298N motor driver
- Task scheduling and multitasking with FreeRTOS

## 🛠️ Hardware Used

- STM32F103C8T6 ("Blue Pill")
- HC-SR04 ultrasonic sensors (x4)
- Bumper switches (x2)
- L298N motor driver
- 2 DC motors + wheels
- Battery pack (11.1 LiPo)
- 2-wheel custom chassis

## ⚙️ Software Architecture

- **RTOS Kernel**: FreeRTOS (manages task switching and scheduling)
- **Tasks**:
  - `SensorTask`: Reads ultrasonic and bumper data periodically
  - `MotorTask`: Handles direction and speed control
- **Inter-task communication** via queues or flags

## 🧠 What I Learned

- Real-time task management with FreeRTOS on STM32
- Efficient sensor integration with closed-loop control
- Interfacing motor drivers and sensors in an RTOS environment

## 🚧 Future Improvements

- Add speed control using rotary encoders
- Improve obstacle recovery strategy
- Incorporate mapping or SLAM algorithms
- Remote control override (e.g., via Bluetooth or Wi-Fi)

