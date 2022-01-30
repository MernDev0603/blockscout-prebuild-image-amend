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

3. deploy local blockscout infrastructure with base ui image container and a database container

<pre>
docker-compose up -d
</pre>

4. check the assets that were replaced by means of mapping in compose/app.yaml file -> services -> blockscout -> volumes

### report the issues to github repository https://github.com/excoincial-blockchain/blockscout-prebuild-image-amend
### do your best to create a docker build image source codes rather than keeping the concept of mapped assets to prebuilt image
