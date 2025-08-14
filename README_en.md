# Huawei Lite Wearable Map App Sample Project
## Development Environment
* DevEco Studio 5.1.0 Release
## Test Environment
### Wearable
| Item | Contents |
| --- | --- |
| Device Name | HUAWEI WATCH 5-25B |
| Model Name | HUAWEI WATCH 5 |
| Model Number | RTS-AL00 |
| HarmonyOS | 5.1.0 |
| Software Version | 5.1.0.205(SP1C900E101R1P100) |
| OpenHarmony Version | OpenHarmony 5.0.1 |
### Lite Wearable
| Item | Contents |
| --- | --- |
| Device Name | HUAWEI WATCH ATM-6D2 |
| Model Name | HUAWEI WATCH ATM |
| Model Number | ATM-B29 |
## Current (August 2025) Lite Wearable Development Considerations
* There are very limited things you can do with Lite Wearable. There are probably more limitations than developers expected. In particular, it is almost impossible to dynamically re-edit a layout once it has been decided on, so it is very difficult to create something elaborate. For this reason, we recommend that you try to create as simple and static a layout as possible.
* The available CSS properties are quite limited. If you create a layout like a web page, you may encounter problems such as the app not working, not being able to display, displaying incorrectly, or not being able to install.
* Negative values cannot be entered for margin-left, margin-right, margin-top, and margin-bottom.
* You can install and run the HAP file on a Lite Wearable device, but you cannot take logs or debug. If you want to log and debug, you have no choice but to use the simulator (Huawei Lite Wearable Simulator) included with DevEco Studio.
* Wearableで動作するからといって、Lite Wearableでも動作するとは限りません。必ずシミュレーター（Huawei Lite Wearable Simulator）で動作確認した上、Lite Wearableの実機で動作を確認しましょう。
* In config.json, we included both liteWearable and wearable in module > deviceType. However, when actually using the project, we recommend splitting the project into two and setting module > deviceType to only liteWearable or wearable. In particular, when installing Wear Engine, the Wearable Wear Engine SDK and the Lite Wearable Wear Engine SDK are different. Installing them simultaneously will prevent the project from building.
## Reference materials
* Lite Smart Watches (https://developer.huawei.com/consumer/en/doc/best-practices/bpta-lite-wearable-guide)
* JavaScript-compatible Web-like Development Paradigm (ArkUI.Lite) (https://developer.huawei.com/consumer/en/doc/harmonyos-references/arkui-js-lite-comp)
* Lifecycle (https://developer.huawei.com/consumer/en/doc/harmonyos-references/js-lite-framework-lifecycle)
* Multilingual support (https://developer.huawei.com/consumer/en/doc/harmonyos-references/js-lite-framework-localization)
* Available CSS properties (https://developer.huawei.com/consumer/en/doc/harmonyos-references/js-lite-common-styles)
* stack tag (https://developer.huawei.com/consumer/en/doc/harmonyos-references/js-lite-components-container-stack)
* div tag (https://developer.huawei.com/consumer/en/doc/harmonyos-references/js-lite-components-container-div)
* image tag (https://developer.huawei.com/consumer/en/doc/harmonyos-references/js-lite-components-basic-image)
* input tag (https://developer.huawei.com/consumer/en/doc/harmonyos-references/js-lite-components-basic-input)
* text tag (https://developer.huawei.com/consumer/en/doc/harmonyos-references/js-lite-components-basic-text)
* @system.router (https://developer.huawei.com/consumer/en/doc/harmonyos-references/js-apis-system-router)
* Wearable App Development (JS) (https://developer.huawei.com/consumer/en/doc/connectivity-Guides/fitnesswatch-dev-0000001051423561)