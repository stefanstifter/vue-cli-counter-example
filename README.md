# vue-cli-counter-example
Just a very simple counter example, to play around with vue-cli.  
Built with vue-cli v4-0-5  

## Deployment

### Prepare local
```
zip -r counter.zip dist/
scp counter.zip user@host:'path/to/public/'
```

### Unzip on staging/production
[enable extended pattern matching operators in shell. painless deletion of all files except .zip file]  
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
