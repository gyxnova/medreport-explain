# MedReport Explain

Multilingual medical report explainer powered by fine-tuned MedGemma.

## What it does

Takes any medical report and explains it in simple language in 5 languages — Hindi, Spanish, Arabic, French, and Bengali.

## Demo

[Add your YouTube link here]

## Model

Fine-tuned `google/medgemma-1.5-4b-it` using QLoRA on MTSamples dataset.

- Training loss: 2.74 → 0.42
- Trainable parameters: 32.8M (1.3% of total)
- Model on HuggingFace: [gyxnova/medreport-explainer](https://huggingface.co/gyxnova/medreport-explainer)

## Languages Supported

| Language | Model |
|---|---|
| Hindi | Helsinki-NLP/opus-mt-en-hi |
| Spanish | Helsinki-NLP/opus-mt-en-es |
| Arabic | Helsinki-NLP/opus-mt-en-ar |
| French | Helsinki-NLP/opus-mt-en-fr |
| Bengali | Helsinki-NLP/opus-mt-en-bn |

## How to run
```bash
pip install transformers peft bitsandbytes gradio sentencepiece torch
```

Then run all cells in `medgemma(3).ipynb`.

## Built for

MedGemma Impact Challenge — Kaggle 2026
