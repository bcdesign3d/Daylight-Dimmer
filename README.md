Daylight Stick Brightness Control with Klipper
Elevate your 3D printing experience with seamless control of your daylight stick's brightness using Klipper! This setup allows you to gradually increase or decrease the light intensity of your daylight stick, all through G-code macros, offering smooth transitions and perfect control over the ambiance.

How it works:
Daylight Stick Brightness Control: The setup utilizes PWM (Pulse Width Modulation) to control the brightness of your daylight stick. This gives you smooth, adjustable brightness levels for precise lighting control during printing.
Gradual Transitions: By modifying the TARGET and STEP parameters, you can control how quickly the brightness ramps up or down, ensuring the transitions are fluid and not abrupt.
Auto Startup: With the DAYLIGHT_ON_STARTUP delayed G-code, your daylight stick will automatically reach the desired brightness level when the printer powers on. No need to manually adjust it—your printer starts ready for the perfect lighting!
Key Features:
Customizable Brightness: Set the target brightness anywhere from 0% to 100%. Default is 30% on startup, but you can adjust it to your needs.
Smooth Brightness Transitions: Choose the step size (default is 5%) to fine-tune the transition speed between brightness levels.
Automated Control: The printer will automatically adjust the brightness on startup using the DAYLIGHT_ON_STARTUP delayed G-code.
Daylight Print Mode: This macro ensures that the daylight stick is adjusted to a balanced 50% brightness when you trigger the print mode.
Setup Instructions:
Pin Configuration: Set your daylight stick to the desired pin (default: PB2). This pin will handle the PWM signal.
G-code Macros: Use DAYLIGHT_ON, DAYLIGHT_OFF, and DAYLIGHT_PRINT macros for manual control or automatic adjustments. You can trigger these macros to gradually adjust the light intensity.
Startup Integration: The DAYLIGHT_ON_STARTUP macro ensures that the brightness is set correctly as soon as the printer powers up.
Example Macros:
DAYLIGHT_ON: Gradually increases the brightness to the desired level.
DAYLIGHT_OFF: Gradually decreases the brightness, turning the light off.
DAYLIGHT_PRINT: Adjusts the brightness to 50%, either by increasing or decreasing the light.
Why Use This Setup?
Perfect Lighting Every Time: Whether you’re setting up your printer or printing, you’ll have the right amount of light, enhancing the printing environment.
Seamless Transitions: The gradual increase/decrease prevents any sudden jumps in brightness, offering a more natural and comfortable experience.
Hands-Free Operation: Set your lighting to adjust automatically on startup, and focus on what really matters—your print jobs!
With this setup, your 3D printer's environment will match your needs, whether you're adjusting for the perfect lighting or letting the printer handle it automatically. Don't just print—print in style with the perfect lighting ambiance every time!
