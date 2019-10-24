# vue-cli-counter-example
built with vue-cli_4-0-5

## prepare for deployment
```
zip -r counter.zip dist/
scp counter.zip ssh-w015487b@w015487b.kasserver.com:'www/htdocs/w015487b/counter.saswebdev.com'
```

## deploy on staging/production
[enable extended pattern matching operators, for easy delete all files except .zip file]  
[`shopt -s extglob`]  
```
rm -rfv !("counter.zip")
unzip counter.zip
mv dist/* .
rm -r dist/ counter.zip
```

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
