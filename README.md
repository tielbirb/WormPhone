<p align="center"><img src="assets/banner.svg" alt="Wormphone banner" width="720"></p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-Android%208.0%2B-3DDC84?logo=android&logoColor=white" alt="Android 8.0+">
  <img src="https://img.shields.io/badge/license-MIT-blue" alt="MIT license">
  <img src="https://img.shields.io/badge/status-early%20%26%20untested-orange" alt="Status: early and untested">
  <img src="https://img.shields.io/badge/made%20with-Kotlin-7F52FF?logo=kotlin&logoColor=white" alt="Kotlin">
  <img src="https://img.shields.io/badge/AI-Anthropic%20%7C%20OpenAI%20%7C%20DeepSeek%20%7C%20Groq-8A2BE2" alt="AI providers">
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen" alt="PRs welcome">
  <img src="https://img.shields.io/badge/pixel%20pets-6%20skins-ff69b4" alt="6 skins">
</p>


# Wormphone

A pixel pet snake that roams your Android screen, over your homescreen and other apps. It chases and eats dots, and you can flick it from one phone to another.

## Features
- Floating pixel pet that moves around on its own and eats the dots that appear
- Drag it, or flick it into another phone running Wormphone
- Skins: Snake, Budgie, Cockatiel, OG Nokia, Minecraft Creeper, Mario (add your own as 8x8 pixel grids)
- Random colour changes for the snake, budgie and creeper skins
- Optional talking: add an API key for Anthropic, OpenAI, DeepSeek or Groq. The provider is picked from the key prefix (`gsk_` = Groq, `sk-ant` = Anthropic, `sk-proj` = OpenAI), otherwise from the in-app provider button
- Works without AI: turn talking off and it just roams and eats

## Install
1. Download the APK from the latest GitHub Actions run (Artifacts > `Wormphone-debug-apk`), or build it in Android Studio.
2. Open Wormphone, tap **Allow drawing over apps** and allow it.
3. Tap **Allow notifications + nearby phones** and accept the prompts.
4. Tap **Start worm**.

## Throwing between phones
Both phones need Wormphone running with the nearby permissions granted. Flick the worm hard and it disappears from your screen and appears on the other one.

## Build
- Android Studio: open the folder, let Gradle sync, press Run.
- GitHub: push the repo and run the **Build Wormphone APK** workflow.

Requires Android 8.0 (API 26) or newer.

## Status
Early and untested. Not yet working: the GGUF model picker only saves a file location and runs nothing, because offline models need llama.cpp built in.

## Skins and trademarks
The Mario, Minecraft Creeper and OG Nokia skins are fan-style pixel art of other companies' characters and designs. They are not covered by this project's license.

## License
MIT
