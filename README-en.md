# pzh-speech
A tiny audio speech (.wav) utility tool (GUI) based on Python2.7+wxPython4.0+PyAudio+Matplotlib+SpeechRecognition(PocketSphinx)+pyttsx3(eSpeak) | 一款支持多引擎的wav格式语音处理小工具（音频录播与波形显示，语音识别，文语合成） 

[![GitHub release](https://img.shields.io/github/release/JayHeng/pzh-py-speech.svg)](https://github.com/JayHeng/pzh-py-speech/releases/latest) [![GitHub commits](https://img.shields.io/github/commits-since/JayHeng/pzh-py-speech/v1.0.0.svg)](https://github.com/JayHeng/pzh-py-speech/compare/v1.0.0...master) [![GitHub license](https://img.shields.io/github/license/JayHeng/pzh-py-speech.svg)](https://github.com/JayHeng/pzh-py-speech/blob/master/LICENSE.txt)

English | [中文](./README.md)

<img src="http://henjay724.com/image/cnblogs/JaysPySPEECH_overview_github.PNG" style="zoom:100%" />

### How to build :
********************
　　First of all, you should install all Non-Python packages listed in [《痞子衡语音处理助手-开发环境搭建》](https://www.cnblogs.com/henjay724/p/9542690.html), then follow below steps:
```text
  1. Install Python2.7.15 x86 version
  2. Confirm that the directory "\Python27\" and "\Python27\Scripts\" are in the system environment variable path after the installation is completed
  3. Double click "\pzh-py-speech\env\do_setup_by_pip.bat" to install the Python library on which pzh-speech depends
  4. Double click "\pzh-py-speech\env\do_pack_by_pyinstaller.bat" to regenerate the pzh-speech.exe
  5. Open "\pzh-py-speech\bin\pzh-speech.exe" to use it
```

### Tool Features :
********************
* View the waveform of selected .wav file
* Record sound from microphone to .wav file (\conv\rec)
* Play selected .wav file
* ASR: Recognize selected .wav file to text (\conv\asr)
* TTS: Translate input text to speech
* TTW: Translate input text to .wav file (\conv\tts)
* Both English and Chinese are supported in ASR,TTS,TTW
* Design detail: [《痞子衡语音处理助手诞生记(全七篇)》](https://www.cnblogs.com/henjay724/p/9541867.html)

Known issues:
* The audio data are all 0x00s if BitDepth is set as 8bits when recording sound (it seems to be PyAudio issue)
* Sometimes Application will hang up if language is set as Chinese when using TTS (it may be MSSpeech_TTS_xxx language package installation issue)

### License :
********************
　　This package is licensed under the BSD three-clause license. See the LICENSE.txt file for details.

Copyright © 2017-2018 Jay Heng.