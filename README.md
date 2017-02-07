# angular-cli

## usage

### make New Project
```bash
docker run --rm -it -v ${PWD}:/usr/src/app -w /usr/src/app yasu2704/angular-cli:6.9-latest ng new newApp
cd newApp
```

if use [yarn](https://yarnpkg.com/)
```bash
docker run --rm -it -v ${PWD}:/usr/src/app -w /usr/src/app yasu2704/angular-cli:6.9-latest ng new newApp --skip-npm
cd newApp
docker run --rm -it -v ${PWD}:/usr/src/app -w /usr/src/app yasu2704/angular-cli:6.9-latest yarn install --ignore-optional
```

### start server
```bash
docker run --rm -it -v ${PWD}:/usr/src/app -w /usr/src/app -p 4200:4200 yasu2704/angular-cli:6.9-latest ng s
```