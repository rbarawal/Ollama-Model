# `Ollama Model`

## Linux

```bash
curl -fsSL https://ollama.com/install.sh | sh

# 1st termux session
ollama serve

# 2nd termux session
ollama run llama3.2:1b
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
