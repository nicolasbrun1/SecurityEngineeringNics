FROM debian:jessie
RUN export node_version="0.10" \
&& apt-get update && apt-get -y install --no-install-recommends nodejs="$node_version" \
 && apt-get clean \
 && rm -rf /var/lib/apt/lists/*
WORKDIR /usr/src/app 
COPY package.json /usr/src/app
WORKDIR /usr/src/app 
RUN npm install node-static@v0.7.11
EXPOSE 65535
CMD ["npm", "start"]
  