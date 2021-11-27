npm init -y                                         # khởi tạo để có package.json
npm i -D webpack webpack-cli                        #cài đặt webpack
npm i node-sass postcss-loader postcss-preset-env   # cài đặt các gói để làm việc với SCSS
npm i sass-loader css-loader cssnano                # cài đặt các gói để làm việc với SCSS, CSS
npm i mini-css-extract-plugin cross-env file-loader # cài đặt các gói để làm việc với SCSS
npm install copy-webpack-plugin                     # cài đặt plugin copy file cho Webpack
npm install npm-watch                               # package giám sát file  thay đổi

note!
nguồn :src
đích :disk


Trong file package.json

"watch": {
      "build":{
        "patterns": ["src"],
        "extensions": "js,scss"
      }
    },
    "scripts": {
      "test": "echo \"Error: no test specified\" && exit 1",
      "build": "webpack",
      "watch": "npm-watch"
    },