
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

## Results

| Configuration | Whisper V3 Large (Base) |
| :--- | :--- |
| *Métriques* | CER / WER |
| **reference_24khz** | **AD** : 0.0268 / 0.0714 <br> **NEB** : 0.0243 / 0.0561 |
| **reference** | **AD** : 0.0268 / 0.0714 <br> **NEB** : 0.0243 / 0.0557 |
| **ZipVoice_fixed_params** | **AD** : 0.1494 / 0.3157 <br> **NEB** : 0.1705 / 0.3584 |
| **ZipVoice** | **AD** : 0.2325 / 0.5001 <br> **NEB** : 0.5743 / 0.8420 |
| **ZipVoice_24khz** | **AD** : 0.2177 / 0.4445 <br> **NEB** : 0.1964 / 0.3576 |

**reference_24khz**: Reference dataset sampled at 24 kHz.
**reference**: Original reference audio sampled at 22,050 Hz.
**ZipVoice_fixed_params**: Inference using the eSpeak tokenizer with the language set to 'fr'.
**ZipVoice**: Inference using the Emilia (English) tokenizer.
**ZipVoice_24khz**: Inference generated using the 24 kHz reference audio, as ZipVoice is configured for 24 kHz.
