# README.md

## 🌍 Multi-Language Text-to-Speech Converter

This program converts text into speech using Google Text-to-Speech (Edge-TTS).\
It supports multiple languages, allows saving and playing audio files, and provides various customization options.

---

## 🇨🇳 多语言文本转语音转换器

本程序使用 Microsoft 文字转语音 (Edge-TTS) 将文本转换为语音。\
它支持多种语言，可保存和播放音频文件，并提供各种自定义选项。

---

## 🇭🇰/🇲🇴 多語言文字轉語音轉換器

本程式使用 Microsoft 文字轉語音 (Edge-TTS) 將文字轉換為語音。\
它支援多種語言，可儲存與播放音訊檔案，並提供各種自訂選項。

---

## 🇪🇸 Conversor de texto a voz multilingüe con Edge-TTS

Este programa convierte texto en voz usando Microsoft Text-to-Speech (Edge-TTS).\
Soporta múltiples idiomas, permite guardar y reproducir archivos de audio y ofrece diversas opciones de personalización。

---

## 🇫🇷 Convertisseur de texte en parole multilingue avec Edge-TTS

Ce programme convertit du texte en parole à l'aide de Microsoft Text-to-Speech (Edge-TTS)。\
Il prend en charge plusieurs langues, permet d'enregistrer et de lire des fichiers audio et offre diverses options de personnalisation。

---

## 🇷🇺 Многоязычный преобразователь текста в речь с Edge-TTS

Эта программа преобразует текст в речь с помощью Microsoft Text-to-Speech (Edge-TTS)。\
Она поддерживает несколько языков, позволяет сохранять и воспроизводить аудиофайлы и предлагает различные параметры настройки。

---

## 🇸🇦 محول النص إلى كلام متعدد اللغات باستخدام Edge-TTS

يقوم هذا البرنامج بتحويل النص إلى كلام باستخدام Microsoft Text-to-Speech (Edge-TTS)。\
وهو يدعم لغات متعددة، ويسمح بحفظ وتشغيل ملفات الصوت، ويقدم خيارات تخصيص متنوعة。

---

## 🇯🇵 多言語対応テキスト音声変換プログラム

このプログラムは、Microsoft Text-to-Speech（Edge-TTS）を使用してテキストを音声に変換します。\
複数の言語に対応し、音声ファイルの保存や再生が可能で、さまざまなカスタマイズオプションを提供します。

---

## 🇰🇷 다국어 텍스트 음성 변환기

이 프로그램은 Microsoft 텍스트 음성 변환(Edge-TTS)을 사용하여 텍스트를 음성으로 변환합니다。\
여러 언어를 지원하며, 오디오 파일 저장 및 재생이 가능하며, 다양한 맞춤 설정 옵션을 제공합니다。

---

## 🇮🇳 Edge-TTS के साथ बहुभाषी टेक्स्ट-टू-स्पीच कन्वर्टर

यह प्रोग्राम Microsoft Text-to-Speech (Edge-TTS) का उपयोग करके टेक्स्ट को आवाज में बदलता है।\
यह कई भाषाओं का समर्थन करता है, ऑडियो फाइलें सहेजने और चलाने की सुविधा देता है और विभिन्न अनुकूलन विकल्प प्रदान करता है।

---

## 🔧 Features & Customization

- ✅ **Multi-language Support** (All UN languages + most spoken languages)
- ✅ **Customizable Speech Speed** (`--speed` option from `0.5x` to `2.0x`)
- ✅ **Audio Format Selection** (`--format mp3/wav/flac/ogg`)
- ✅ **Automatic Multi-Language Playback** (No argument runs all languages)
- ✅ **Save & Playback Options** (`--no-save`, `--no-play`)

## 🔹 How to Install and Run the Program

### 📥 Cloning the Repository
To get started, clone the repository from GitHub using the following command:

```sh
git clone https://github.com/juyujing/multilang-tts.git
cd multilang-tts
```

### 🛠 Setting Up the Conda or Pip Environment

To use this project, you need to set up the appropriate environment using either **Conda** or **pip**.

---

## **🔹 Using Conda (Recommended)**
Make sure you have [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) installed. Then, create and activate the environment using:

```sh
conda env create -f environment.yaml
conda activate tts
```

If your Conda configuration uses `.yml` instead of `.yaml`, use:

```sh
conda env create -f environment.yml
conda activate tts
```

To update the environment if dependencies change:

```sh
conda env update -f environment.yaml
```

To remove the environment if needed:

```sh
conda env remove -n tts
```

---

## **🔹 Using Pip & Virtual Environment**
If you prefer to use **pip** instead of Conda, you can set up a virtual environment manually.

### **Step 1: Create a Virtual Environment**

```sh
python -m venv tts_env
```

### **Step 2: Activate the Virtual Environment**

#### **On macOS/Linux**
```sh
source tts_env/bin/activate
```

#### **On Windows**
```sh
tts_env\Scripts\activate
```

### **Step 3: Install Dependencies**

```sh
pip install -r requirements.txt
```

To update dependencies later:

```sh
pip install --upgrade -r requirements.txt
```

To deactivate the virtual environment:

```sh
deactivate
```

To remove the virtual environment completely:

```sh
rm -rf tts_env  # macOS/Linux
rd /s /q tts_env  # Windows
```


### 🚀 Running the Program

#### 🎧 Running with Default Settings
Simply run:

```sh
python tts.py
```

This will play and save a combined multi-language audio file.

#### 📖 Viewing the Help Menu
To see all available options:

```sh
python tts.py -h
```

This will display detailed descriptions of the supported parameters, available in multiple languages.

#### 📌 Example Commands

```bash
python tts.py -t "Hello, world" -l en --speed 1.5
python tts.py -t "你好，世界" -l zh-cn --format wav
python tts.py -t "Bonjour le monde" -l fr
python tts.py --lang es -o ./output
```

#### 🎙 Running with Custom Parameters
To generate and play English speech from a custom text:

```sh
python tts.py -t "Hello, this is a test speech" -l en
```

To save an audio file in `.wav` format without playing it:

```sh
python tts.py -t "Testing speech synthesis" -l en -f wav --no-play
```

To generate speech in Chinese and increase the speed:

```sh
python tts.py -t "你好，这是一个测试语音" -l zh-cn --speed 1.5
```

To generate a combined multilingual speech file without saving:

```sh
python tts.py --no-save
```

### 🔄 Supported Parameters

#### 🎵 **Language Selection (`-l / --lang`)**
Choose the speech language. If not specified, all default languages will be used.

Example:
```sh
python tts.py -t "Bonjour tout le monde" -l fr
```

#### 🔊 **Text Input (`-t / --text`)**
Specify the text to convert to speech.

Example:
```sh
python tts.py -t "This is a sample text" -l en
```

#### ⏩ **Playback Speed (`--speed`)**
Adjust the playback speed. Default: `1.2` | Allowed range: `0.5 - 2.0`

Example:
```sh
python tts.py -t "Fast speech example" --speed 1.8
```

#### 🎼 **Audio Format (`-f / --format`)**
Choose the output format. Supported formats: `mp3`, `wav`, `flac`, `ogg`

Example:
```sh
python tts.py -t "Speech in different formats" -f wav
```

#### ✅ **Save & Playback Options (`--no-save`, `--no-play`)**
- `--no-save`: Prevents saving the audio file.
- `--no-play`: Disables automatic playback.

Example:
```sh
python tts.py -t "Silent generation" --no-play --no-save
```

### 🛠 Troubleshooting

#### 🛑 **Permission Denied when Saving Files**
If you encounter a `PermissionError`, try running the command with elevated privileges:
```sh
sudo python tts.py
```
Or specify an output directory where you have write access:
```sh
python tts.py -o ~/Downloads
```

#### 🔊 **Audio Not Playing**
If the generated audio is not playing, ensure that `pygame` is correctly initialized and that your system supports audio playback.

Try restarting `pygame`:
```sh
python -c "import pygame; pygame.mixer.quit(); pygame.mixer.init()"
```

Or play the audio manually:
```sh
python -c "import pygame; pygame.mixer.init(); pygame.mixer.music.load('tts_en_xxxx.mp3'); pygame.mixer.music.play()"
```

#### 🔄 **Reinstall Dependencies**
If you face issues with missing packages, try reinstalling the dependencies:
```sh
pip install -r requirements.txt
```
Or in Conda:
```sh
conda env update --file environment.yaml --prune
```

### 📜 License
This project is licensed under the MIT License. Feel free to use and modify it for your needs.
