## Custom `Modelfile` from `sitemap.xml`

```bash
curl -fsSL https://ollama.com/install.sh | sh

# 1st termux session
ollama serve

# 2nd termux session
python app.py
python generate.py

ollama create blogforge -f ./Modelfile
OLLAMA_USE_CUDA=1 ollama run blogforge
```

## Sample commands:

```bash
~/Scrapper$ ollama create blogforge -f ./Modelfile
gathering model components 
using existing layer sha256:6a0746a1ec1aef3e7ec53868f220ff6e389f6f8ef87a01d77c96807de94ca2aa 
using existing layer sha256:4fa551d4f938f68b8c1e6afa9d28befb70e3f33f75d0753248d530364aeea40f 
using existing layer sha256:8ab4849b038cf0abc5b1c9b8ee1443dca6b93a045c2272180d985126eb40bf6f 
creating new layer sha256:7f031c93f3da9489828d2d7fd3245fcea63dfa7dbe14afb547e41eab664442a5 
using existing layer sha256:8c495976fa8f1ed6de92488512ccec55ddbe17c21ec3a6af45eff0075f33269b 
writing manifest 
success

~/Scrapper$ ollama run blogforge
>>> hi
Hi! It's nice to meet you. Is there something I can help you with, or would you like to chat?

>>> tell me about latest blogs
Based on the extracted files, here are some of the latest blogs from Vicks:

1. **Top Physical Exercises for Better Health** - Published on January 17, 2025, this blog explores various physical exercises that can improve overall 
health and well-being.
2. **The Maha Kumbh Festival: A Celebration of Faith and Culture** - Released on January 15, 2025, this blog delves into the history, significance, and 
cultural aspects of the Maha Kumbh festival.
3. **Climate Change 2024: Understanding the Impact and Mitigating Measures** - Published on January 18, 2025, this blog discusses the current state of 
climate change, its effects, and potential solutions to mitigate its impact.

These blogs showcase Vicks' expertise in various topics, including health, culture, and environmental issues. If you're interested in learning more 
about these subjects or other related topics, feel free to ask!

>>> >>> Send a message (/? for help)
[1]+  Stopped                 ollama run blogforge
```
