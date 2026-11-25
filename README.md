[README.md](https://github.com/user-attachments/files/35433486/README.md)
# PodBridge

**PodBridge 0.1.0-alpha5 · Build 5** is a root-free Android companion for AirPods 

This is a personal test build. Bluetooth behavior and feature availability depend on the AirPods model, firmware, and Android audio route. The Android APK and physical AirPods behavior still need device testing.

## Screenshots

### Main screen

Check the connection and battery, switch listening modes, and open **Listen**. The menu beside Listen contains Help and Settings.

<img src="podbridge-home.png" alt="PodBridge Build 5 home screen with AirPods battery and listening modes" width="240">

### Listen through Pixel

Select the Bluetooth headphones, start the Pixel microphone, and place the phone near the person speaking. Start with a low headphone volume.

<img src="listen-through-pixel.png" alt="Listening screen with selected AirPods and Start Pixel microphone button" width="240">

### Listen with Pixel in pocket

Select **Use AirPods Transparency** to hear through the microphones in the AirPods. Once Transparency is active, the Pixel can be locked or put away.

<img src="listen-with-pixel-in-pocket.png" alt="Listening screen with Use AirPods Transparency button" width="240">

## What it does

- Shows reported AirPods battery levels and provides Transparency, Noise Cancellation, Adaptive, and Off controls when supported.
- Provides a Pixel microphone listening option with Boost, Speech clarity, and Left / right balance controls.
- Requests AirPods Transparency for pocket listening through the earbuds' microphones.
- Exposes compatible AirPods settings such as ear detection, press-and-hold controls, call controls, Personalized Volume, and Conversational Awareness. Available controls vary by model and firmware.
- Runs without root, an account, or an Internet permission on the phone.

For a personalized hearing profile on compatible AirPods Pro 2 or 3, use Hearing Assistance on a supported iPhone or iPad to take Apple's Hearing Test or enter a professional audiogram. The AirPods retain that profile for pocket listening. PodBridge's manual tuning applies to the Pixel microphone stream. PodBridge does not run a hearing test or create an audiogram.

## Requirements

- Android 17 or later on an ARM64 device. 
- Compatible AirPods paired and connected in Android Bluetooth settings.
- Nearby devices permission for the AirPods connection. Pixel microphone listening also requests microphone permission.
```

## Privacy and limitations

Pixel listening processes microphone audio in memory and saves the three tuning preferences on the device. Pocket listening uses the AirPods' microphones. 

Apple firmware updates, Find My network, Siri, Apple device switching, and Apple's spatial audio renderer are outside this build. Hearing assistance and noise control should be checked with the actual AirPods. A digital output limiter does not measure acoustic exposure.

## License and credits

Based on Librepods by Kavish Devar and contributors. PodBridge source changes are provided under **GPL-3.0-or-later**. See `LICENSE` in the source archive. AirPods is an Apple trademark. PodBridge is independent of Apple, Google, and the LibrePods project.
