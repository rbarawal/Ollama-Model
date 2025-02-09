># `Ollama Model`
>
>      Yes, Ollama works offline with custom model for your website sitemap.xml
>
>![image](https://github.com/user-attachments/assets/c57eb4d4-6a60-46f8-82a6-847990ab0988)

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
