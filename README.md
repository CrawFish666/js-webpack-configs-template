##Getting Started
1. Clone the repo
```sh
git clone https://github.com/CrawFish666/js-webpack-configs-template.git
```
2. Install NPM packages
```sh
npm install
```
3.  Start a project
```sh
npm run dev - running webpack with devServer
npm run build - running production project
```
### Description folder project

* **dist**
* **src** - folder for development
* * **fonts** - fonts
* * **img** - folder for images/icons
* *    **js** - folder for js
* * * index.js - main script where use all imports, first is import scss
* * **scss** - folder for css/scss styles
* * * fonts.scss - import fonts with `googleFonts` or `@font-face`
* * * main.scss - import `styleReset.scss` and all scss modules and `fonts.scss`
* * * resetStyle.scss - reset styles
* * **index.html**
* .gitignore
* package.json
* package-lock.json
* webpack.dev.js - dev config
* webpack.prod.js - production config
```
