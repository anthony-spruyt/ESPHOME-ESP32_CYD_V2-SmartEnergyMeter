# ESPHOME-ESP32_CYD_V2-SmartEnergyMeter Solar Monitor Configuration

![20241121_190408](https://github.com/user-attachments/assets/98b5d0d1-35e8-4e53-99f0-1f9d7d111d01)

## Description

The **ESP32 Solar Monitor** is an advanced configuration for ESPHome that integrates an **ESP32-2432S028R** display with **Home Assistant**. This project allows real-time monitoring of your photovoltaic system data, including solar production, household consumption, grid import/export, and battery status.

The graphical interface is developed with **LVGL**, offering a modern and interactive design with touch support.

## Features

- **Solar Production**: Real-time monitoring of generated power.
- **Household Consumption**: Display of energy consumed by the house.
- **Grid Import/Export**: Data on imported or exported energy.
- **Battery Status**: Charge percentage and charging/discharging status.
- **Touch Interface**: Smooth navigation between different screens.
- **Graphs and Indicators**: Progress bars and dynamic icons to represent data.

## System Requirements

- **Hardware**:
  - ESP32-2432S028R with TFT display and touchscreen.
  - Photovoltaic inverter configured in Home Assistant.
  - Sensors for production, consumption, and battery.

- **Software**:
  - [ESPHome](https://esphome.io/) configured on the local network.
  - Font `materialdesignicons-webfont.ttf` placed in the `fonts/` directory.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourname/esp32-solar-monitor.git
   cd esp32-solar-monitor

2. **Prepare necessary files**:
   - Copy the font `materialdesignicons-webfont.ttf` to the `fonts/` directory.
   - Configure the `secrets.yaml` file with your Wi-Fi credentials and API keys.

3. **Upload configuration to ESPHome**:
   - Modify necessary parameters in the YAML file (device name, Home Assistant entity IDs, etc.).
   - Upload the configuration to the ESP32 device via the ESPHome interface.

4. **Configure Home Assistant**:
   - Ensure sensors are correctly configured in Home Assistant to provide the required data.

## Usage

After installation, the interface will display:

- **Solar Production**: Current value in watts, with a progress bar.
- **Household Consumption**: Energy consumed by the house.
- **Grid**: Imported or exported energy.
- **Battery**: Charge status and energy flow (charging/discharging).

You can navigate between screens using the interactive touch menu at the bottom of the display.

## Customizations

- **Font and Styles**: Modify colors and sizes in the `lvgl.theme` section of the YAML file.
- **Home Assistant Sensors**: Update entity IDs in the `sensor` section to match your configuration.
- **Navigation and Screens**: Customize layout and content in the `lvgl.pages` sections.

## Contribute

Contributions are welcome! To report issues or suggest improvements, open an [issue](https://github.com/simone7121/ESPHOME-ESP32_CYD_V2-SmartEnergyMeter/issues) or submit a pull request.

## License

This project is distributed under the **GPL V3** license. For more details, see the [LICENSE](LICENSE) file.

## Author

Developed with passion by **[Simone7121]**.

For more information or questions, contact [info@simonedanna.it](mailto:info@simonedanna.it).
