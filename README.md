# matchUP
A maker education service platform, WormIT Co., Ltd.'s first product collaborate with Seeed Studio.

Base on Lantern, an isomorphic web application built with modern technologies, which contains basic functionality, fundamental design and workable architecture.
Good to be used to create your project quickly.

The architecture design was already done for **isomorphic**.
The views and frontend stuffs which are implemented with **React** can be rendered on server-side and client-side both and using the same configuration of routes.
The good news is, there is no need to learn anti-pattern flux framework（e.g., redux）for isomorphic.
Lantern provided an easy way for developers who are already familar with flux pattern.

Besides, the callback hell are not there anymore.
The **generator** is widely used in this project, which is the new technology in new version of ECMAScript（JavaScript）for flow control.
The Backend is using generator with **Koa** web framework, and frontend is using generator in **Flux** framework as well.

Not only technique things, but also UI design is pretty cool in Lantern project.
The framework that **Semantic UI** bring us fantastic frontend user interface, even better than bootstrap and other UI framework.

## 使用技術
### HTML, CSS and JavaScript
* [ECMAScript 6/7（JavaScript 6/7）](http://www.ecmascript.org/)

### Front-End Web UI Frameworks
* [Semantic UI](http://semantic-ui.com/)

### Front-End JavaScript Frameworks
* [React](https://facebook.github.io/react/)
* [Flux](https://facebook.github.io/flux/)

### Server-side Development
* [Express](http://expressjs.com/)
* [Koa](http://koajs.com/)
* [Node.js](https://nodejs.org/en/)

### Database
* [MongoDB](https://www.mongodb.org/)

### Tools
#### NPM - npm is the package manager for whatever
* Official website: https://www.npmjs.com/

#### webpack - MODULE BUNDLER 
* Official website: https://webpack.github.io/
* Github: https://github.com/webpack/webpack

#### PM2 - Advanced, production process manager for Node.js
* Official website: http://pm2.keymetrics.io/
* Github: https://github.com/Unitech/pm2

#### Babel
* Official website: https://babeljs.io/
* Github: https://github.com/babel/babel

## Documentation
See Fred's [Wiki](https://github.com/cfsghost/lantern/wiki) for more information.

## Installation
In order to support ES6+ and using a lots of new technologies (ex, generator and classes), Node.js 0.12+ or io.js is required. Once you have such environment, you can start to install modules needed via **NPM**.
```
npm install
```

Then you can use webpack to compile and combine all of frontend source code for service.
```
webpack
```

Finally, you can start this web service：
```
node app.js dev
```

## Features
* Fast to setup and easy to customize
* UI is pretty cool and fantasic
* Widely use ES6 and ES7+（Generator and classes）
* Isomorphic Architecture
* Support permission management
* Support user database system
* Support Hot loading without webpack-dev-server
* Support i18n for multiple language
* Support third-party Authorization（Facebook/Github/Google/Linkedin）

## Dependencies
* Node.js 0.12+ or io.js
* Koa web framework
* MongoDB
* Fluky - Event-based framework for flux data flow pattern
* babel 5 - Used to support ES6/ES7+
* React v0.14+
* react-router 1.0.0+ - router for React
* Semantic UI - Front-end UI toolkit
* Webpack
* Passport

## License
* Licensed under the ? License

## Authors
Copyright(c) 2015 James Pang &lt;ling.tien5846@gmail.com&gt;

Copyright(c) 2015 Julie Huang &lt;<chunghui0904@gmail.com>&gt;

## How to run matchUP on your local machine（OS X）
Download source code to your local machine
```
https://www.dropbox.com/home?preview=matchUP.tar.gz
```

打包 + 壓縮 文件夾
```
tar -czvf ./matchUP.tar.gz ./matchUP/
```

解壓縮 文件夾
```
tar -zxvf ./matchUP.tar.gz
```

安裝 NVM（Node Version Manager）
```
https://github.com/creationix/nvm
```
```
git clone git@github.com:creationix/nvm.git ~/.nvm
```
```
echo "~/.nvm/nvm.sh" >> ~/.bashrc
```
```
nvm install v4.2.1
```

使用 npm 安裝缺少的模組
```
npm install xxx
```

執行
```
node app.js
```

End
```
http://localhost:3001/
```

## Server info

### China
```
http://imatchup.cc/
```
Deploy Server
* IP address：[123.59.83.143](123.59.83.143)
* Password：Julings@82101?

### USA
```
http://matchup.top/
```
Compile Server
* IP address：[54.200.125.101](54.200.125.101)

Deploy Server
* IP address：[54.200.181.10](54.200.181.10) 

## SCP（Secure Copy）
查看本機 IP address
```
http://dir.twseo.org/ip-check.php
```

從本機複製到遠端伺服器
* sudo scp ./*.tar.gz root@123.59.83.143:/root

從遠端伺服器複製到本機
* sudo scp root@123.59.83.143:/root/*.tar.gz .

## Deploy steps
```
tar -zxvf ./*.tar.gz
```

```
cd *.git
```

```
. ~/.nvm/nvm.sh
```

```
nvm use v4.1.2
```

```
webpack -p
```

```
pm2 restart Genuino
```

## 更改 root 密碼
```
passwd
```
