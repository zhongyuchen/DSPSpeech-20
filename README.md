# DSPSpeech-20

[![MIT license](https://img.shields.io/badge/license-MIT-e78ac3.svg)](https://mit-license.org)

A speech dataset of 20 isolated words each with 720 recordings from 36 individuals

## Size

* Number of audio files: `36 individuals * 20 words each individual * 20 times each word = 14400 recordings`
* Size of a single file: 66 KB
* Total size: 943.2 MB

## Description

Each audio file is a recording of an isolated word. The audio files are named as `speech_data/<ID>/<ID>-<LABEL>-<ROUND>.wav`.

### <ID>

Audio files with the same `<ID>` are contributed by the same individual.

### <LABEL>

There is a corresponding isolated word for each `<LABEL>` from `00` to `19`.

|  00    |   01  |    02  |   03  |    04    |    05 |   06   |  07   |    08  |    09    |
| ------ | ------ | ------ | ------- | ------- |------ | ------ | ------ | ------- | ------- |
| 数字    | 语音   | 语言   | 识别     | 中国    | 总工    | 北京   | 背景   | 上海     | 商行    |

|  10    |   11  |    12  |   13  |    14    |    15 |   16   |  17   |    18  |    19    |
| ------ | ------ | ------ | ------- | ------- |------ | ------ | ------ | ------- | ------- |
| 复旦    | 饭店   | Speech | Speaker | Signal  |Process | Print | Open   | Close   | Project |

### <ROUND>

For each individual, each isolated word is recorded for 20 times, which is indicated by `<ROUND>` from `01` to `20`.

## Parameters

| Format | AudioFormat | NumChannels | SampleRate | BitRate | BitDepth | length |
| ------ | ------ | ------ | ------- | ------- | ------- | ------- |
| `.wav` | PCM | 1 | 16 kHz | 256 kbps | 16 bits | ~2 s |

These are the important parameters regarding the audio files. 
If you'd like to get more information about the audio files, 
you can look closely at the header of the files.
While doing so, keep in mind that it's __little-endian__ format!
