# Local deployment of blockscout for EXL-mainnet

requirements:
- ability to install and use docker and docker-compose on local
- basic 

1. install docker and docker-compose

2. clone git repository and browse into the folder

<pre>
git clone https://github.com/excoincial-blockchain/blockscout-prebuild-image-amend
cd blockscout-prebuild-image-amend
</pre>

3. change permissions for ssl files
<pre>
sudo chown 999:999 data/blockscout/ssl/server.key data/blockscout/ssl/server.crt
sudo chmod 600 data/blockscout/ssl/server.key data/blockscout/ssl/server.crt
</pre>

4. deploy local blockscout infrastructure with base ui image container and a database container

<pre>
docker-compose up -d
</pre>

5. check the assets that were replaced by means of mapping in compose/app.yaml file -> services -> blockscout -> volumes

## screenshot of page available at http://localhost:4000
![home page](https://raw.githubusercontent.com/excoincial-blockchain/blockscout-prebuild-image-amend/master/local-home-screenshot.png)

### report the issues to github repository https://github.com/excoincial-blockchain/blockscout-prebuild-image-amend
### do your best to create a docker build image source codes rather than keeping the concept of mapped assets to prebuilt image
