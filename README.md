
This repository provides a set of audio samples from the **Blizzard 2023 segmented corpus**. The samples are categorized as follows:

- **Reference**: Original segmented audio from Corbora.
- **ZipVoice**: Inference generated at 22,000 Hz.
- **ZipVoice 24kHz**: Inference generated at 24,000 Hz.
- **Fine-tuned ZipVoice**: Output from the model fine-tuned on 22,000 Hz audio.



## Directory Structure
Structure:
```
collected_samples/
├── AD/
│   ├── reference/
│   ├── zipVoice/
│   ├── zipVoicekhz24/
│   └── zipVoic_fintuned/
└── NEB/
    ├── reference/
    ├── zipVoice/
    ├── zipVoicekhz24/
    └── zipVoic_fintuned/
```