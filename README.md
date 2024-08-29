# Etekcity Fitness Scale BLE Integration for Home Assistant

This custom integration allows you to connect your Etekcity Bluetooth Low Energy (BLE) fitness scale to Home Assistant. It provides real-time weight measurements directly in your Home Assistant instance, without requiring an internet connection or the VeSync app.

## Features

- Automatic discovery of Etekcity BLE fitness scales
- Real-time weight measurements
- Customizable display units (kg, lb, st)
- Direct Bluetooth communication (no internet or VeSync app required)

**Note:** Currently, only weight measurement is supported. Future updates may include support for impedance measurements and/or impedance-based body composition estimates.

[![Buy Me A Coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ronnnnnnn)

## Installation

### HACS (Recommended)

1. Ensure that [HACS](https://hacs.xyz/) is installed in your Home Assistant instance.
2. In the HACS panel, go to "Integrations".
3. Click the "+" button and search for "Etekcity Fitness Scale BLE".
4. Click "Install" on the Etekcity Fitness Scale BLE integration.
5. Restart Home Assistant.

### Manual Installation

1. Copy the `etekcity_fitness_scale_ble` folder to your Home Assistant's `custom_components` directory.
2. Restart Home Assistant.

## Configuration

1. In Home Assistant, go to "Configuration" > "Integrations".
2. Click the "+" button to add a new integration.
3. Search for "Etekcity Fitness Scale BLE" and select it.
4. Follow the configuration steps to add your scale.

## Supported Devices

This integration has been tested with the following Etekcity scale models:

- [ESF-551 (Smart Fitness Scale)](https://etekcity.com/products/smart-fitness-scale-esf551)

Other Etekcity BLE fitness scale models may work but have not been tested. If you try it with a different model, please let me know whether it works or not.

## Troubleshooting

- Ensure that your Home Assistant instance has Bluetooth capabilities and that the Bluetooth integration is properly set up.
- Make sure your scale is within range of your Home Assistant device.
- If you encounter any issues, please check the Home Assistant logs for more information.

### Raspberry Pi 4 and other Linux machines using BlueZ

If you encounter a `org.bluez.Error.InProgress` error, try the following in `bluetoothctl`:

```
power off
power on
scan on
```

(See [this GitHub issue](https://github.com/home-assistant/core/issues/76186#issuecomment-1204954485) for more information)

## Support the Project

If you find this unofficial project helpful, consider buying me a coffee! Your support helps maintain and improve this integration.

[![Buy Me A Coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ronnnnnnn)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Disclaimer

This integration is not official. It is not endorsed by, directly affiliated with, maintained, authorized, or sponsored by Etekcity, VeSync Co., Ltd., or any of their affiliates or subsidiaries. All product and company names are the registered trademarks of their original owners. The use of any trade name or trademark is for identification and reference purposes only and does not imply any association with the trademark holder of their product brand.

Use this integration at your own risk.