# Voice-Gulliver

🌍 [한국어](docs/README.kor.md) ∙ [English](docs/README.eng.md) ∙ [日本語](docs/README.jpn.md)

[![GitHub License](https://img.shields.io/github/license/abus-aikorea/voice-gulliver)](LICENSE)
[![GitHub Release](https://img.shields.io/github/v/release/abus-aikorea/voice-gulliver)](https://github.com/abus-aikorea/voice-gulliver/releases )

The best gradient web-ui for asr, translation and tts. Easy one click installation. Fully portable.


## Introduction
* Voice Gulliver is an integrated solution for **subtitles**, **translation**, and **dubbing**. 
* Add multilingual subtitles to your video with Voice Gulliver. Expansion into the global market is possible!
* You watch world news every morning? Then, try using the live translation function. It supports real-time translation, just like what you see on YouTube.
* Voice Gulliver is equipped with **Vocal Remover** provided by UVR5 and Meta's **Demucs** engine. 
* Voice Gulliver uses **OpenAI Whisper** and **Microsoft Azure AI**.      
* Voice Gulliver can be easily installed with **one click** and provides Gradio Web-UI. 
* Experience the highest level of **On-Device AI Voice** technology.


## Main function

* `VOD` tab
  - Provides integrated environment for YouTube downloader, noise removal, subtitles, translation, and dubbing
  - All video/audio formats supported by ffmpeg can be used
  - Selectable output audio format (wav, flac, mp3)
  - Speech recognition and subtitle creation for 100 languages
  - Select subtitle creation options suitable for PC performance (Whisper Model & Compute Type)
  - The BGM and sound effects from the original video remain the same in the dubbed video.
  - Supports speed, volume, and pitch adjustment of dubbing voice  
  
<p align="center">
  <img style="width: 90%; height: 90%" src="docs/images/main_page.eng.png?raw=true" alt=""/>
</p>  


* `Live` tab
  - Real-time voice recognition & translation support
  - Select audio input source such as Mic, Speaker, etc.
  - Provides the ability to save captured audio, recognized subtitles, and translated subtitles

* `Batch` tab
  - Batch process large amounts of files



## Features
* You can download YouTube videos (mp4, webm) and save them as audio files (mp3, wav, flac).
* You can increase the accuracy of voice recognition by removing noise and separating vocals. **MDX-Net** and Meta's **Demucs** are used.
* **One-click installation**. Once installed, you can use it **permanently** at no additional cost. (※ Free version has **30 minute limit** on usage time)
* Provides **Web-UI**. Google Chrome browser is recommended.


## Execution environment
* OS: Windows 10/11 (64bits) **※ Linux and Mac OS are not supported.**
* CPU: Intel processor 2GHz or higher (or equivalent compatible)
* RAM: 4GB or more
* HDD: At least 20GB of free space during installation
* GPU: **NVIDIA** graphics card supporting CUDA 12.1 recommended. VRAM 4GB or more. 8GB or more recommended.
* Internet connection required (installation and translation work)


## Install and run

### step 1. Package preparation
* A. Paid version
    + Unzip the compressed file (**voice-gulliver-x.zip**) included in the USB to an appropriate location on your computer.
    + Or, copy the already unzipped folder (**voice-gulliver-x**) to an appropriate location on your computer.

* B. Free version
  + [![GitHub Release](https://img.shields.io/github/v/release/abus-aikorea/voice-gulliver)](https://github.com/abus-aikorea/voice-gulliver/ Download and unzip the latest release (**Source code (zip)**) from 
  + Or, download source code with git clone
    
```bash
git clone https://github.com/abus-aikorea/voice-gulliver.git
```

### step 2. Install and run the program
1. Run `configure.bat`
   - Install ffmpeg and CUDA (if using NVIDIA GPU) on Windows. 
   - You only need to run it the first time.
2. Run `start.bat`
   - Start Voice-Gulliver. Web-UI will run automatically. 
   - When running for the first time, Voice-Gulliver is installed first. 
   - Voice-Gulliver installation requires an Internet connection, and depending on the system, installation may take more than an hour. 
   - Never close the Windows-Command window during installation.
   - If a problem occurs during installation, delete the installer_files folder and run start.bat again.
#### If Browser does not run automatically
- Close the Windows-Commnad window and run start.bat again.
- Run the browser directly and enter the address displayed in the Windows-Command window (e.g. **http://127.0.0.1:7892**) in the address bar.


### Run screen

https://github.com/abus-aikorea/voice-gulliver/assets/161691694/bb7dd2f2-9863-49e3-bd3e-59b0b8315fca


### step 3. Uninstall program
* Run `uninstall.bat`:
  - Remove the installer_files folder.
  - Remove ffmepg and CUDA packages installed on Windows (if selected)

* Voice-Gulliver has **portable** installation as standard. To uninstall the program, deleting the installation folder is sufficient.


## caution
When Windows Defender mistakenly recognizes a batch file as a Trojan, this is often called a 'False Positive'. To solve this problem, you can go through the following steps:

1. File exception handling: In Windows Defender, you can set certain files or processes to skip security scanning. To do this, follow the steps below:
   * Click the ‘Start’ button and go to ‘Settings’.
   * Click ‘Update & Security’.
   * Select ‘Windows Security’ and go to ‘Virus & threat protection’.
   * Click ‘Manage Virus & Threat Protection Settings’.
   * Select 'Add exception' in 'Virus & threat protection settings'.
   * Select 'File or Folder', find the batch file in question and add it as an exception.
2. Temporarily disable Windows Defender: This may be a temporary solution. However, you must be careful when using this method as it may expose your computer to other threats.
3. Report the problem to anti-virus software: If you are sure that the file is not a Trojan horse, you can report it to Microsoft as a False Positive. Microsoft will review this and take any necessary action.


## Contact us
* e-mail: <abus.aikorea@gmail.com>
* homepage(Korean): <https://abuskorea.imweb.me>
* 네이버 스마트스토어 (S/W): <https://smartstore.naver.com/abus/products/10385660040>
* 네이버 스마트스토어 (Solution): <https://smartstore.naver.com/abus/products/10298346364>
* Coupang(Korean): <https://www.coupang.com/vp/products/7875503674>
* Amazon(US): <https://www.amazon.com/dp/B0D5H8Z4FL>
* Amazon(Japan): <https://www.amazon.co.jp/dp/B0CTHT2JH3>


## YouTube
* Product Information: <https://youtu.be/heEN4UIQLjc>
* Automatic Subtitle∙Translation: <https://youtu.be/uQ14hoEiI4c?si=Io9K_vIDYyeu9Z8_>
* Home Karaoke: <https://youtube.com/playlist?list=PLwx5dnMDVC9bVxfGo58U-R-w3fUHqwiD6&si=TZBh5AFjcr7_dyiI>
  


## Credits
* FacebookResearch Demucs: <https://github.com/facebookresearch/demucs>
* yt-dlp: <https://github.com/yt-dlp/yt-dlp>
* gradio: <https://github.com/gradio-app/gradio>


## Copyright
<p align="center">
  <img src="docs/images/ABUS_logo.jpg" width="100" height="100"> by [ABUS](https://abuskorea.imweb.me)
</p>
