
This repository provides a set of audio samples from the **Blizzard 2023 segmented corpus**. The samples are categorized as follows:

- **Reference**: Original segmented audio from Corbora.
- **Reference 24kHz**: Reference recordings at 24,000 Hz.
- **ZipVoice**: Inference generated at 22,000 Hz.
- **ZipVoice 24kHz**: Inference generated at 24,000 Hz.
- **ZipVoice Fixed Params**: Inference generated with fixed parameters.
- **Fine-tuned ZipVoice**: Output from the model fine-tuned on 22,000 Hz audio.



## Directory Structure
Structure:
```
collected_samples/
├── AD/
│   ├── reference/
│   ├── reference_24khz/
│   ├── zipVoice/
│   ├── zipVoicekhz24/
│   ├── zipVoice_fixed_params/
│   └── zipVoic_fintuned/
└── NEB/
    ├── reference/
    ├── reference_24khz/
    ├── zipVoice/
    ├── zipVoicekhz24/
    ├── zipVoice_fixed_params/
    └── zipVoic_fintuned/
```