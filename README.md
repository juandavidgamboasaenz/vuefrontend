# vuefrontend

## Project setup
```
npm install
```

## Deploy into GitPages 

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

### Initialazing repository for GitHub pages

for this process we must add a vue.config.js file in the root of our project. Here, we want to configure the publicPath (which also edits the webpack publicPath) to route all static assets to the proper path.

```javascript
module.exports = {
  publicPath: process.env.NODE_ENV === "production" ? "/REPO_NAME/" : "/",
};
```

Now to run and update the gitHub pages use this command. Add the dist changes and commit them into the subtree.

Also we need that dist is not included in the .gitignore in the new branch created.

```bash
  git add dist && git commit -m 'adding dist subtree'
```

then we need to push the changes into the subtree try using:

```bash 
  git subtree push --prefix dist origin gh-pages
```
