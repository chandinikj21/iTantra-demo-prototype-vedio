# iTantra

## Project Description
iTantra is an offline-first, speech-driven communication system built for disaster zones, remote military outposts, and low-bandwidth radio links where internet and cellular networks fail. It runs entirely on-device — no cloud, no internet dependency — turning any Android phone into a resilient voice transceiver over ultra-low-bitrate channels (300 bps–2.4 kbps). Instead of transmitting raw audio or plain text, iTantra converts speech into a compact semantic packet, protects it with hybrid error correction, and reconstructs it as natural speech — in the sender's own voice — on the receiving end. Built for Smart India Hackathon 2026, Problem Statement SIH26173.

## Features
- Fully offline, on-device speech-to-text and text-to-speech across 22 Indian languages
- Meaning-based compression — reduces each message to 5–15 bytes instead of full audio or raw text
- Reed-Solomon + LDPC hybrid forward error correction for reliable delivery over noisy, low-bitrate radio links
- Priority emergency override — critical alerts instantly interrupt playback and force maximum volume
- Speaker-preserving voice reconstruction using zero-shot voice cloning, so the receiver hears the sender's real voice
- Bluetooth/Wi-Fi Direct mesh relay as a backup path when the primary radio link drops
- Runs on low-end Android hardware (tested target: ~₹8,000 devices, 2–3 GB RAM)

## Technologies Used
- Kotlin (Android application)
- TensorFlow Lite (on-device inference, INT8/INT4 quantization, XNNPACK delegate)
- AI4Bharat IndicConformer v2 (speech-to-text)
- VITS2 / Matcha-TTS (speech synthesis and voice cloning)
- Reed-Solomon + LDPC (forward error correction)
- HTML, CSS, JavaScript (project landing page / prototype showcase)

## Demo Video
[▶️ Watch Project Demo](https://youtu.be/nM24F2wmXgY)

## How to Run
1. Clone the repository: `git clone [YOUR_REPO_LINK]`
2. Open the project in Android Studio and let Gradle sync dependencies.
3. Connect an Android device (Android 8+) or start an emulator.
4. Build and run the app; grant microphone and Bluetooth/Wi-Fi permissions when prompted.
5. On two devices, open the app as Sender and Receiver to test the full speech-to-radio-to-speech pipeline.

## Team Members
- [Chandini K J]
- [Chandana K J]
- [Dedeepya S]
- [Malavika Mukunda]
- [Amrutha S]
- [Druthi N]

