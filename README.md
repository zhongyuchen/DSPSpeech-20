# DSPSpeech-20

[![MIT license](https://img.shields.io/badge/license-MIT-e78ac3.svg)](https://mit-license.org)

A speech dataset of 20 isolated words each with 680 recordings from 34 individuals

## Status

* Vocabulary: __20 words__ in the following table
* Speaker: __34 individuals__
* Amount: __13,599 recordings__ (20 of each word per speaker)
* Size of a single file: __66 KB__
* Uncompressed package size: __891.5 MB__
* Compressed package size: __521.4 MB__

## Download

* Baidu Cloud
```
链接:https://pan.baidu.com/s/1EAon920Ko6aoMx4uAttmcQ  密码:x15n
```

* GitHub repo
```
git clone https://github.com/zhongyuchen/DSPSpeech-20.git
```

## Vocabulary

Each audio file is a recording of an isolated word. The audio files are named as `speech_data/{speakerID}/{speakerID}-{label}-{index}.wav`. For example, `speech_data/16307130194/16307130194-12-16.wav` is the `16`th word `Speech` recorded by speaker `16307130194`.

|  00    |   01  |    02  |   03  |    04    |    05 |   06   |  07   |    08  |    09    |
| ------ | ------ | ------ | ------- | ------- |------ | ------ | ------ | ------- | ------- |
| 数字    | 语音   | 语言   | 识别     | 中国    | 总工    | 北京   | 背景   | 上海     | 商行    |

|  10    |   11  |    12  |   13  |    14    |    15 |   16   |  17   |    18  |    19    |
| ------ | ------ | ------ | ------- | ------- |------ | ------ | ------ | ------- | ------- |
| 复旦    | 饭店   | Speech | Speaker | Signal  |Process | Print | Open   | Close   | Project |

## Parameters

| Format | AudioFormat | NumChannels | SampleRate | BitRate | BitDepth | length |
| ------ | ------ | ------ | ------- | ------- | ------- | ------- |
| `.wav` | PCM | 1 | 16 kHz | 256 kbps | 16 bits | ~2 s |

These are the important parameters regarding the audio files. 
If you'd like to get more information about the audio files, 
you can look closely at the header of the files.
While doing so, keep in mind that it's __little-endian__ format!

## Application

* [speech-classification](https://github.com/zhongyuchen/speech-classification): CNN and VGG speech classification with interactive website for testing

## Source

The recordings are contributed by 34 students of _Digital Signal Processing Spring 2019_ and recorded on this [website](https://zhongyuchen.github.io/audio-collector/). Check [here](https://github.com/zhongyuchen/audio-collector) for the implementation of the dataset collecting website.
