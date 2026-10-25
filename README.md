# MuseGPT

A music-generation fine-tuning project by Dhruv Saini, released on Hugging Face under my earlier handle, `oof-baroomf`.

I fine-tuned Falcon-40B with LoRA to generate music in ABC notation. Falcon-40B is the upstream base language model from the Technology Innovation Institute; the music adapters are my fine-tuning work.

- [Trained adapters, tokenizer and model card](https://huggingface.co/oof-baroomf/MuseGPT)
- [Cleaned 35k music dataset](https://huggingface.co/datasets/oof-baroomf/MuseGPT-35k-cleaned)
- [43k dataset referenced by the model card](https://huggingface.co/datasets/oof-baroomf/MuseGPT-43k)
- [Upstream Falcon-40B](https://huggingface.co/tiiuae/falcon-40b)
- [Video demonstration](https://drive.google.com/file/d/1FhOEWrFZQKOaWhtqX9v4ZyAvTKfGtIrm/view)

## Release contents

The trained adapter weights, adapter configuration, tokenizer files and training arguments are on Hugging Face. The model card documents 4-bit NF4 quantization and the PEFT version used.

This GitHub repository is an index to that release. The original training notebook is not currently archived here. The datasets contain music encoded as text; the musical compositions and the underlying Falcon model are not claims of original authorship.
