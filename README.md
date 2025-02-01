# `Ollama Model`

## Linux

```bash
curl -fsSL https://ollama.com/install.sh | sh

# 1st termux session
ollama serve

# 2nd termux session
ollama create mario -f ./Modelfile
ollama run mario
```

## Termux

```bash
pkg install tur-repo
pkg install ollama

# 1st termux session
ollama serve

# 2nd termux session
ollama run llama3.2:1b
```
