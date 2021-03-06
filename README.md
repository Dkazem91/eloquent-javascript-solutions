# Shell
<img src="https://s-media-cache-ak0.pinimg.com/originals/48/ff/a3/48ffa351eec2f1bb021b15f05f372bdb.jpg" width="40%" height="40%">

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
- Vagrant/Virtual Box

## how to install for development
Clone the repository to your local machine and then install dependencies once inside the dolphin directory.
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

## Deploying Locally
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



