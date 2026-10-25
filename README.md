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

## Historical training source

[Recovered July 2023 music fine-tuning notebook](training/Music-finetuning-2023.ipynb)

This is my music adaptation of Hugging Face's [Falcon/QLoRA training example](https://huggingface.co/blog/falcon#fine-tuning-resources). It uses my music-text dataset and Falcon-40B. The general training scaffold comes from the upstream example, which is credited in the notebook. Original code cells are preserved; cell outputs and runtime metadata have been removed.

This earlier experiment is not an exact recipe for the published adapter: its LoRA dropout is 0.1, while the release records 0.05. The exact final training notebook has not yet been recovered. The historical notebook installed the then-current packages without version pins, so its original TRL/PEFT APIs may need adaptation on a modern environment.

The trained release remains on Hugging Face. The datasets contain music encoded as text; the musical compositions and the underlying Falcon model are not claims of original authorship.
