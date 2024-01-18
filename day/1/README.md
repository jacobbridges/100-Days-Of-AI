# Day 1

My first day of learning AI was to load some models. I did not want to spend money on OpenAI's API, so the logical starting point was finding some models to use locally.

I will be using the following models in my learning:

- [Tiny Llama](https://github.com/jzhang38/TinyLlama) - Can be loaded on most devices, and the mascot on this one is adorable. 🦙
- [mistral-7b-openorca](https://huggingface.co/Open-Orca/Mistral-7B-OpenOrca) - Was highly rated on gpt4all.io, and I love orcas.
- [whisper](https://github.com/openai/whisper) - OpenAI's whisper model, used to translate audio into text.

## Notebooks

### 1-load-tiny-llama-model.ipynb

Fetch the tiny llama model from HuggingFace, then utilizes it in a chat setting. Just confirming the model loads with no errors.

### 2-load-mistral-7b-model.ipynb

Load the mistral-7b-openorca model and submits a simple prompt. Assumes the mistral-7b-openorca model has already been downloaded to the `models` in the root of the repo.