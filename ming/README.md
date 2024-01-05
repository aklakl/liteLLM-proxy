# liteLLM Proxy Server: 50+ LLM Models, Error Handling, Caching

1. Clone liteLLM repository to your local machine:
   ```
   git clone https://github.com/BerriAI/liteLLM-proxy
   ```
2. Install the required dependencies using pip
   ```
   python3.11 -m venv myenv
   source myenv/bin/activate
   deactivate

   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```
3. (optional)Set your LiteLLM proxy master key
   ```
   os.environ['LITELLM_PROXY_MASTER_KEY]` = "YOUR_LITELLM_PROXY_MASTER_KEY"
   or
   set LITELLM_PROXY_MASTER_KEY in your .env file
   ```
4. Set your LLM API keys
   ```
   os.environ['OPENAI_API_KEY]` = "YOUR_API_KEY"
   or
   set OPENAI_API_KEY in your .env file
   ```
5. Run the server:
   ```
   python3.11 main.py
   ```

# Resources
```

git clone https://github.com/BerriAI/liteLLM-proxy
git clone https://github.com/BerriAI/litellm

litellm-proxy/proxy_server.py
litellm-proxy/proxy_cli.py
refer:https://github.com/canada4663/litellm/blob/98abecf124317a772a9a3ced57ebd118e5823173/docs/my-website/docs/proxy_server.md?plain=1#L510



Colab 
!pip install litellm google-generativeai
!pip install fastapi nest-asyncio pyngrok uvicorn
!litellm --create_proxy
cd litellm-proxy
!export PALM_API_KEY={YOUR_PALM_API_KEY}
!ngrok config add-authtoken 2aFTceY6HsXFymUchvjYRsmxw71_P74qKHeJtQf6nDpWo9P5


demo instruction refer:https://youtu.be/J2DYaP6VWVQ?t=171
demo colab refer:https://colab.research.google.com/drive/1hKopUBlqh13Erke_kQtNgr79N86kH_WZ?usp=sharing
AutoGen with Ollama/LiteLLM - Each Agent With Its OWN LOCAL MODEL (Tutorial):https://youtu.be/y7wMTwJN7rA





========
docker pull ubuntu | docker pull python

docker container prune
docker image prune
docker run -d -it -p 22:22 --name mingubuntu ubuntu:latest 
docker exec -it mingubuntu /bin/bash
apt install python3.11
apt install python3.11-full
apt install python3-pip
apt install git-all
apt install curl

refer:https://www.linuxcapable.com/how-to-install-python-3-11-on-ubuntu-linux/

/home/ming/liteLLM-proxy

docker commit mingubuntu
docker tag 47f8faec2e70 ming_python311_litellm_proxy

```