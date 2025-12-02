# 🎧 EasyEffects Convolver Presets for Lenovo V15

A set of Impulse Response (`.irs`) files designed to replicate the sound profiles of **Dolby Audio** on Linux systems using the **EasyEffects** application (formerly PulseEffects).

---

## 💻 Supported Models

These files are specifically generated for the **Lenovo V15 (First Generation)** series. While tuned for the models below, they may be compatible with others sharing the same speaker hardware:

* **V15-ADA** (AMD)
* **V15-IIL** (Intel)

## ✨ Included Presets

The following four Dolby Audio profiles were captured as individual Impulse Response files:

| Preset File Name | Dolby Profile | Description | Recommended Use Case |
| :--- | :--- | :--- | :--- |
| `V15movie.irs` | Movie | Enhanced surround effects and clear dialogue. | Watching films and video streaming. |
| `V15music.irs` | Music | Balanced frequency response optimized for clarity and punch. | General music listening. |
| `V15games.irs` | Game | Boosted effects and directional audio for immersion. | Playing games. |
| `V15voice.irs` | Voice | Maximizes speech clarity and reduces background noise. | Video conferencing (Zoom, Meet, etc.). |

## 🔧 Installation and Setup

To use these presets, you must have the **EasyEffects** audio processing application installed on your Linux distribution (e.g., from your distribution's package manager or Flathub).

### 1. Import the Files

1.  Download all `.irs` files from the repository's source directory.
2.  Open **EasyEffects**.
3.  Ensure the **Convolver** plugin is added and active in your main pipeline.

### 2. Configure the Convolver

1.  In the Convolver plugin interface, locate the **Impulse** settings.
2.  Click the **"Import impulse"** button at the top of the modal window.
3.  Navigate to and select your desired `.irs` file (e.g., `V15music.irs`).

> [!WARNING]
> **Important Gain Adjustment:** Impulse Responses can significantly alter volume levels. **Always** reduce the **Input Gain** and/or **Output Gain** (e.g., start at **-6.0 dB** or lower) within the Convolver to prevent digital clipping and speaker distortion. You can fine-tune them later.

## ❓ How These Files Were Generated

The Impulse Response files were created by capturing the system's output on a Lenovo V15-ADA while the official Windows Dolby Audio drivers were active.

* **Input Signal:** A digital impulse sound from [AudioCheck](https://www.audiocheck.net/testtones_impulse.php) was used (44.1kHz).
* **Recording Method:** The audio output was recorded back into **Audacity** for each of the four Dolby presets (48kHz).
* **Sampling Rate:** The resulting files are recorded at a **48 kHz** sample rate.

---

## 🛑 Disclaimer

* **Use at Your Own Risk (UAYOR):** These files are provided as-is. While they aim to replicate the factory sound, results may vary depending on your specific kernel, audio drivers, and EasyEffects configuration.
* **Clipping & Distortion:** Users are responsible for monitoring their sound levels. Excessive gain may damage your speakers.
