# 🌟 Daylight Stick Brightness Control with Klipper

This project enables you to integrate smooth, customizable lighting control for your daylight stick directly into your Klipper setup. Perfect for ensuring optimal visibility and creating a professional printing environment.

---

## 🚀 Features

- **Customizable Brightness**: Adjust the brightness level between 0% and 100%. The default startup brightness is set to 30%, but you can easily modify it.
- **Smooth Transitions**: Achieve seamless brightness changes with customizable step sizes, avoiding abrupt light changes.
- **Automatic Startup**: Automatically sets the desired brightness level when the printer starts.
- **Daylight Print Mode**: Conveniently adjust the brightness to 50% for balanced lighting during print operations.

---

## 🛠️ How It Works

### 📂 Configuration Overview

1. **`[output_pin]`**: This section defines the hardware pin connected to your daylight stick and sets up PWM control.
2. **`[delayed_gcode]`**: Runs the `DAYLIGHT_ON` macro during printer startup, setting the initial brightness level.
3. **Macros**:
   - `DAYLIGHT_ON`: Gradually increases the brightness to a target level.
   - `DAYLIGHT_OFF`: Gradually decreases the brightness to 0%.
   - `DAYLIGHT_PRINT`: Adjusts the brightness to 50%, whether increasing or decreasing as needed.

---

## 📥 Installation

1. **Download the Configuration**: Save the provided `daylight.cfg` file to your Klipper configuration folder.
2. **Edit the File**: Open `daylight.cfg` and update the pin configuration under `[output_pin daylight_pwm]` to match the port you use to control your daylight stick.
3. **Include in Printer Config**: Add the following line to your `printer.cfg` to include the daylight control configuration:
   
   [include daylight.cfg]

---

## 📝 Example Use Cases

- **Startup Lighting**: Ensure the printer area is well-lit when Klipper initializes.
- **Balanced Print Lighting**: Automatically adjust brightness to 50% for optimal visibility during prints.
- **Dynamic Control**: Manually increase or decrease brightness as needed during operation.

---

## 🔗 Notes and Tips

- **Pin Configuration**: Ensure the pin specified in `[output_pin daylight_pwm]` supports PWM.
- **Fine-Tuning**: Adjust the `step` and `cycle_time` values to control the smoothness and speed of brightness changes.
- **Safety First**: Always verify your hardware’s power handling capabilities to prevent overloads.

---

With this configuration, your Klipper-powered 3D printer will not only perform exceptionally but look great doing so! 🎉
