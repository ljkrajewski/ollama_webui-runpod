# ollama_webui-runpod

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
