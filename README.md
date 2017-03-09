# Supported tags and respective `Dockerfile` links
* [`7.7`](https://github.com/yasu2704/angular-cli/blob/master/7.7-latest/Dockerfile),[`7.7-latest`](https://github.com/yasu2704/angular-cli/blob/master/7.7-latest/Dockerfile),[`latest`](https://github.com/yasu2704/angular-cli/blob/master/7.7-latest/Dockerfile) [(7.7-latest/Dockerfile)](https://github.com/yasu2704/angular-cli/blob/master/7.7-latest/Dockerfile)
* [`7.6`](https://github.com/yasu2704/angular-cli/blob/master/7.6-latest/Dockerfile),[`7.6-latest`](https://github.com/yasu2704/angular-cli/blob/master/7.6-latest/Dockerfile) [(7.6-latest/Dockerfile)](https://github.com/yasu2704/angular-cli/blob/master/7.6-latest/Dockerfile)
* [`7.5`](https://github.com/yasu2704/angular-cli/blob/master/7.5-latest/Dockerfile),[`7.5-latest`](https://github.com/yasu2704/angular-cli/blob/master/7.5-latest/Dockerfile) [(7.5-latest/Dockerfile)](https://github.com/yasu2704/angular-cli/blob/master/7.5-latest/Dockerfile)
* [`6.10`](https://github.com/yasu2704/angular-cli/blob/master/6.10-latest/Dockerfile),[`6.10-latest`](https://github.com/yasu2704/angular-cli/blob/master/6.10-latest/Dockerfile) [(6.10-latest/Dockerfile)](https://github.com/yasu2704/angular-cli/blob/master/6.10-latest/Dockerfile)
* [`6.9`](https://github.com/yasu2704/angular-cli/blob/master/6.9-latest/Dockerfile),[`6.9-latest`](https://github.com/yasu2704/angular-cli/blob/master/6.9-latest/Dockerfile) [(6.9-latest/Dockerfile)](https://github.com/yasu2704/angular-cli/blob/master/6.9-latest/Dockerfile)

## usage

### make New Project
```bash
docker run --rm -it -v ${PWD}:/usr/src/app -w /usr/src/app yasu2704/angular-cli:6.10 ng new newApp
cd newApp
```
---
if use [yarn](https://yarnpkg.com/)
```bash
docker run --rm -it -v ${PWD}:/usr/src/app -w /usr/src/app yasu2704/angular-cli:6.10 ng new newApp --skip-npm
cd newApp
docker run --rm -it -v ${PWD}:/usr/src/app -w /usr/src/app yasu2704/angular-cli:6.10 yarn install --ignore-optional
```
---
### start server
```bash
docker run --rm -it -v ${PWD}:/usr/src/app -w /usr/src/app -p 4200:4200 yasu2704/angular-cli:6.10 ng s
```
