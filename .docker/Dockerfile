FROM nikolaik/python-nodejs:python3.10-nodejs17
WORKDIR /discordgsm
RUN curl -s  https://codeload.github.com/DiscordGSM/DiscordGSM/zip/refs/tags/v1.9.2 > source.zip \ 
  && unzip source.zip \
  && cd DiscordGSM-1.9.2 \
  && pip install -r requirements.txt \
  && npm install -g gamedig \
cmd ["python3", "DiscordGSM-1.9.2/bot.py"]
