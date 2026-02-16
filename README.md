# 🎵 Custom Sounds

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Firefox](https://img.shields.io/badge/Firefox-Add--on-orange.svg)](https://addons.mozilla.org/es-ES/firefox/addon/custom-sounds/)
[![Chromium](https://img.shields.io/badge/Chromium-Extension-4285F4.svg)](https://chrome.google.com/webstore)

### Available languages
[![Language: English](https://img.shields.io/badge/Language-English-blue.svg)](README.md) [![Idioma: Español](https://img.shields.io/badge/Idioma-Español-red.svg)](README.es.md)

**Custom Sounds** is an extension designed to personalize your web browsing experience by adding sound effects to different actions within your browser.

---

## 🖼️ Images
### Settings Page
![Settings Page](/images/options_page.png "Settings page")

### Event Customization Modal
![Modal](/images/modal.png "Event modal")

---

## ✨ Features
- 🔊 **Custom Sounds:** currently, you can assign sounds to:
    * ➕ Open/Close tabs.
    * ⌨️ Keystrokes.

- 🛠️ **Simple Configuration:** intuitive interface to manage your audio files.

- 🚀 **Lightweight:** optimized to ensure no impact on browser performance.

## ⏭️ ~~Upcoming Features~~ Completed Features!!!
- 🎚️ **Volume Control:** because only you should decide how fast you want to destroy your ears.

- ⌨️ **Multiple keys, same sound:** so you can assign your favorite sounds to your keyboard.

## 💻 Technologies Used
* JavaScript (WebExtensionAPI): for background logic and browser events.

* HTML: for the options page.

* CSS (Tailwind CSS): for the interface design.

## ⬇️ Installation

### For Users
[**Now available on AMO**](https://addons.mozilla.org/en-US/firefox/addon/custom-sounds/) or, if you prefer, you can install it manually by downloading the distribution .zip for your browser from the [Latest Release](https://github.com/kirutre/custom_sounds/releases/latest) or by following the development steps.

### Developer Guide (Manual Installation)
If you want to modify the extension or contribute to the code, follow these steps to set up your local environment.

1. **Clone this repository**
    ```bash
    git clone https://github.com/Kirutre/custom_sounds.git

    cd custom_sounds
    ```

2. **Styles Management (Tailwind CSS)**

    This extension uses Tailwind CSS for the interface. The `output.css` file is already included in the repository so the extension works immediately, but if you make design changes, you will need to recompile it.

    #### Recompile `output.css`
    1. Download the CLI executable for your operating system from [Tailwind CSS Releases](https://github.com/tailwindlabs/tailwindcss/releases/tag/v4.1.18).

    2. Place the executable in the project root and rename it to `tailwindcss-cli`.

    3. Run the following command to compile and watch changes in real-time.

    ```bash
    ./tailwindcss-cli -i ./options/input.css -o ./options/output.css --watch --minify
    ```

> [!TIP]
> If you have Node.js installed, you can avoid downloading the binary manually by using:

```bash
npx @tailwindcss/cli -i ./options/input.css -o ./options/output.css --watch --minify
```

3. **Load for testing**
    + In Firefox
        1. Rename `manifest-firefox.json` to `manifest.json`.

        2. Open Firefox and type `about:debugging` in the address bar.

        3. Click on "This Firefox".

        4. Click on "Load Temporary Add-on...".

        5. Select the `manifest.json` file inside the project folder.
    
    + In Chromium
        1. Rename `manifest-chromium.json` to `manifest.json`.

        2. Open your Chromium-based browser and type `chrome://extensions/` in the address bar.

        3. Enable "Developer Mode".

        4. Click on "Load unpacked".

        5. Select the project root folder (where `manifest.json` is located).

## 🤝 Contributing
Contributions are what make software better, and I’m excited to see what you have to offer!

Please read the [**Contributing Guidelines**](CONTRIBUTING.md) to get started. Whether it's fixing a bug or suggesting a crazy new sound trigger, all help is welcome!

## 📝 License
Distributed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## 📬 Contact
Kirutre - [GitHub](https://github.com/kirutre)

Kirutre - contact.kirutre+firefox@gmail.com

Project Link: https://github.com/Kirutre/custom_sounds