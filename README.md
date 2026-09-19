# ollama_webui-runpod

## Pick a Model
[Can I Run AI](https://www.canirun.ai/):  Tests your computer and suggests what you can run.

## Running Qwen3.8-27B-Uncensored

Pick a 23GB+ VRAM pod on [Runpod](https://runpod.ai) (or wherever). See the [Ollama library page](https://ollama.com/orcarouter/Qwen3.8-27B-Uncensored) if you want a smaller model.

Already done buy someone else, and it works well.

- Template: Ollama with Open WebUI - PyTorch 2.7.0 CUDA 12.x
- Image:    sombi/ollama-open-webui:base-torch2.7.0-cu124

In a web terminal,
```bash
apt update
apt install zstd
pkill ollama
curl -fsSL https://ollama.com/install.sh | sh
ollama serve
ollama pull orcarouter/Qwen3.8-27B-Uncensored:q6_K   #or whatever model you choose
```
then click on the OpenWebUI link in the runpod VM.

## Uncensored models
- [maxwellb/gemma4-12b-it-oym:bf16](https://ollama.com/maxwellb/gemma4-12b-it-oym)
- [orcarouter/Qwen3.8-27B-Uncensored:q6_K](https://ollama.com/orcarouter/Qwen3.8-27B-Uncensored)
