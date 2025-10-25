#  LED Blink using STM32F446RE (STM32CubeMX + STM32CubeIDE)

🛠️ Description

A simple embedded project that toggles an LED ON and OFF every second using STM32F446RE.
This project is created using STM32CubeMX (for pin configuration and clock setup) and built in STM32CubeIDE.

⚙️ Hardware Setup

Microcontroller: STM32F446RE

Development Board: NUCLEO-F446RE (or bare MCU)

LED Connection:

LED → GPIO Pin (Configured in CubeMX, e.g., PA5 or user-defined pin)

Series Resistor: 220Ω – 330Ω

LED Cathode → GND

🧩 Software Setup

Toolchain: STM32CubeIDE

Code Generator: STM32CubeMX

Clock Source: HSI (High-Speed Internal, 16 MHz) with PLL enabled

System Clock: 180 MHz

Delay: HAL_Delay(1000)

🧠 How It Works

MCU initializes HAL, clock, and GPIOs.

The LED pin is configured as push-pull output.

Inside the main loop, the LED toggles every second using HAL_Delay(1000).

📸 Example Output

LED blinks with a 1-second interval.

You can verify with an oscilloscope or by observing LED blinking rate.
