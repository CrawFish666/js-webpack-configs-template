## Getting Started
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
* * * index.js - main script for index.html
* * **scss** - folder for css/scss styles
* * * fonts.scss - import fonts with `googleFonts` or `@font-face`
* * * main.scss - import `styleReset.scss` and all scss modules and `fonts.scss`
* * * resetStyle.scss - reset styles
* * * common.scss - have only scss styles which common uses in other pages(BEM block and etc)
* * * index.scss - import common.css if you need, main.scss and have css styles for index.html
* * **index.html**
* .gitignore
* package.json
* package-lock.json
* webpack.dev.js - dev config
* webpack.prod.js - production config
## What's new?
$${\color{green}v2.0.0}$$
```
1. Добавил чанки, для дробления общих css стилей и js функций на общие файлы
2. Добавил подключение мульти HTML страниц
3. Теперь точки входа берутся по названиям HTML страниц. Т.е. index.html - точка входа index.js
4. В production SVG,png,jpg,gif теперь пережимаются и имеют меньший размер без заметной потери качества
5. В production png,jpg переделываются в webp и имеют более меньший размер
```
$${\color{green}v1.0.0}$$
```
1. Добавил 2 конфига сборки: production and dev
```
## What's next?
- [ ] В production mode после пережимки картинок + превращения в webp сделать автоподключение коробочки picture. Это позволит браузерам, которые поддерживают webp подгружать webp картинки вместо JPG/PNG. Будет более быстрая загрузка. Возможно сделать это же и для css
- [ ] В dev mode добавить пережимку картинок + конвертацию в webp + опционально подключение коробочки picture в html, и возможно css
