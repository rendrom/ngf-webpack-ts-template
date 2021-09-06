# NGF webpack template for Typescript

Basic template for NextGIS Frontend web application with submodule development

## Installation

```bash
npm i
# build prod version
npm run prod
# start development server
npm start
```

Add submodule to simplify the development process

```bash
git submodule update --init
# get latest version on nextgis_frontend submodule
cd ./@nextgis
git checkout master
git pull origin master
```

## Docker

```bash
docker build -t ngf-template:latest -f docker/Dockerfile .
docker run -it -p 8080:80 --rm --name ngf-template ngf-template:latest
```
