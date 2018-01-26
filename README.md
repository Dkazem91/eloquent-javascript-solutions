# Dolphin

![alt text](https://vdk.colornumbers.ru/wa-data/public/shop/products/48/17/11748/images/8080/8080.900.jpg "Dolphin")

Dolphin is an administrative console and the web front-end side of Sagetalk.

It uses an isomorphic stack which utilizes:
- ReactJs
- Redux
- NodeJS
- WebPack
- Babel

## Pre-Requisites
### operating system:
- Linux – Ubuntu 14.04+
- Windows - ? 
- packages - @sagebots/dolphin

## how to install for development
```shell
git clone https://github.com/sage-bots/dolphin.git
```
```shell
npm install
```

any additional required dependencies asked to install can be done with 

```shell
-npm install -g <program name>
```

### Troubleshooting 
If errors arise from outdated dependency versions while installing:
- make sure OS is up-to-date.
- update or rebuild npm:
```shell
npm update
```
```shell
npm rebuild
```
- delete node_modules folder and reinstall
```shell
rm -rf node_modules/
npm install
```

## deploying locally
### Mongo
- Create /data/db for mongo with user writable permissions
```shell
sudo mkdir -p /data/db
sudo chmod -R go+w /data/db
```
- Run `mongod` in one terminal and `mongo` in another:

### Dolphin and Mermaid
- navigate to the mermaid and dolphin directories on your local machine and run: 
```shell
npm run dev
```
#### Notes
-  Dolphin will be available on http://localhost:3000/
- create a login on http://localhost:3000/register?token=my-token
- use this login at port 3000 for access to rest of website. 
- mermaid will be on port 3030



