# SmartThings-Home-Assistant-Connect

## THIS PROJECT IS NO LONGER BEING MAINTAINED

This SmartApp allows you to connect your existing Home Assistant devices to SmartThings. The main reason I created this is because I was frustrated by the limitations of the emulated_hue component, specifically with Google Home. With your Home Assistant devices available in SmartThings, you can connect your SmartThings hub to Alexa/Google Home instead of relying on emulated_hue.

## Supported Devices, Features, and Limitations
Currently cover, light, script, and switch device types are supported.

- **cover** - Like emulated_hue, cover devices are treated like lights, so you have to say "turn on the shades" to open them, etc. Also supports setting the position.
- **light** - All lights are treated like colored bulbs. You are able to use voice control to set the color.
- **script** - Treated like a switch.
- **switch** - Basic on and off. Surprise, surprise.

You can use the **smartthings_name** attribute in Home Assistant to set a custom name for your device in SmartThings. Otherwise, **friendly_name** will be used.

## Installation
1. Install and publish the Smart App in the Smart App IDE using "Create via code".
1. Under Settings in the Smart App IDE, add the following App Settings:
   - **token** - a long-lived access token, created in your Home Assistant user account
   - **hassUrl** - your Home Assistant URL
1. Install and publish all Device Handlers in the Device Handler IDE using "Create via code".
1. Open the SmartThings app on your phone, and install the Home Assistant Connect SmartApp from the Marketplace (under My Apps).
1. Select all the Home Assistant devices you would like to connect to SmartThings.
1. You should now be able to control your Home Assistant devices from SmartThings!
