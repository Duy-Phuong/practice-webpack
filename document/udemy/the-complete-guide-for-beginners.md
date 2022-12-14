
- [Resources](#resources)
- [1. Introduction](#1-introduction)
  - [1. Introduction](#1-introduction-1)
  - [2. What you need for this course](#2-what-you-need-for-this-course)
- [2. Initial Setup and Integrating Webpack](#2-initial-setup-and-integrating-webpack)
  - [1. Why Do We Need Webpack](#1-why-do-we-need-webpack)
  - [2. Setting Up Our Application](#2-setting-up-our-application)
  - [3. Install Webpack And Integrate It With NPM](#3-install-webpack-and-integrate-it-with-npm)
  - [Custom webpack configuration](#custom-webpack-configuration)
  - [4. Small Note about Github Repository.html](#4-small-note-about-github-repositoryhtml)
  - [4.1 Github Repository.html](#41-github-repositoryhtml)
  - [5. Integrating Webpack Into Our JS Application](#5-integrating-webpack-into-our-js-application)
- [Asset modules](#asset-modules)
  - [Handle images](#handle-images)
  - [publicPath](#publicpath)
  - [Asset/inline Module Type](#assetinline-module-type)
  - [General Asset Type](#general-asset-type)
  - [Asset/source Module Type](#assetsource-module-type)
- [3. Loaders](#3-loaders)
  - [1. What Is Webpack Loader](#1-what-is-webpack-loader)
  - [2. Handling Images With Webpack](#2-handling-images-with-webpack)
  - [3. Handling Images With Webpack. How To Use publicPath](#3-handling-images-with-webpack-how-to-use-publicpath)
  - [4. Handling CSS With Webpack](#4-handling-css-with-webpack)
  - [5. Handling SASS](#5-handling-sass)
  - [6. Using Latest JavaScript Features With Babel 7](#6-using-latest-javascript-features-with-babel-7)
- [4. Plugins](#4-plugins)
  - [1. What Is Webpack Plugin](#1-what-is-webpack-plugin)
  - [2. Minification Of The Resulting Webpack Bundle](#2-minification-of-the-resulting-webpack-bundle)
  - [3. Extracting CSS Into a Separate Bundle With mini-css-extract-plugin, Part 1](#3-extracting-css-into-a-separate-bundle-with-mini-css-extract-plugin-part-1)
  - [4. Extracting CSS Into a Separate Bundle, Part 2](#4-extracting-css-into-a-separate-bundle-part-2)
  - [5. Browser Caching](#5-browser-caching)
  - [6. How To Clean Dist Folder Before Generating New Bundles](#6-how-to-clean-dist-folder-before-generating-new-bundles)
  - [7. Generating HTML Files Automatically During Webpack Build Process](#7-generating-html-files-automatically-during-webpack-build-process)
  - [8. Customizing Generated HTML Files](#8-customizing-generated-html-files)
  - [9. Integration with Handlebars](#9-integration-with-handlebars)
  - [10. More Webpack Plugins](#10-more-webpack-plugins)
  - [](#)
- [5. Production vs Development Builds](#5-production-vs-development-builds)
  - [1. Introduction](#1-introduction-2)
  - [2. Mode](#2-mode)
  - [3. Managing Webpack Config for Production and Development Use Cases](#3-managing-webpack-config-for-production-and-development-use-cases)
  - [4. Faster Development with webpack dev server](#4-faster-development-with-webpack-dev-server)
  - [5. Cleaning Up A Bit](#5-cleaning-up-a-bit)
- [6. Multiple Page Applications](#6-multiple-page-applications)
  - [1. Introduction](#1-introduction-3)
  - [2. Creating KiwiImage Component](#2-creating-kiwiimage-component)
  - [3. Code Splitting in Webpack Multiple JS and CSS Bundles](#3-code-splitting-in-webpack-multiple-js-and-css-bundles)
  - [4. How To Generate Multiple HTML Files](#4-how-to-generate-multiple-html-files)
  - [5. Extracting Common Dependencies While Code Splitting](#5-extracting-common-dependencies-while-code-splitting)
  - [6. Setting Custom Options for Code Splitting](#6-setting-custom-options-for-code-splitting)
  - [7. How To Setup Development Environment For Multiple Page Application](#7-how-to-setup-development-environment-for-multiple-page-application)
- [7. Webpack Integration With Node And Express](#7-webpack-integration-with-node-and-express)
  - [1. Introduction](#1-introduction-4)
  - [2. Getting Code for Single Page Application.html](#2-getting-code-for-single-page-applicationhtml)
  - [3. Integrating Express Into Our Application](#3-integrating-express-into-our-application)
  - [4. Serving HTML Pages via Express](#4-serving-html-pages-via-express)
  - [5. Handling JS and CSS via Express](#5-handling-js-and-css-via-express)
  - [6. Getting Code for Multiple Page Application.html](#6-getting-code-for-multiple-page-applicationhtml)
  - [7. Integrating Express.js Into A Multiple Page Application](#7-integrating-expressjs-into-a-multiple-page-application)
- [8. Integration with jQuery](#8-integration-with-jquery)
  - [1. Getting the Source Code.html](#1-getting-the-source-codehtml)
  - [2. Integration with jQuery](#2-integration-with-jquery)
- [9. Using Custom Fonts with Webpack](#9-using-custom-fonts-with-webpack)
  - [1. Using Custom Fonts with Webpack](#1-using-custom-fonts-with-webpack)
- [10. Integration with Bootstrap](#10-integration-with-bootstrap)
  - [1. Using Bootstrap with Webpack](#1-using-bootstrap-with-webpack)
  - [2. 2nd Method Of Importing CSS From Bootstrap](#2-2nd-method-of-importing-css-from-bootstrap)
- [11. Using FontAwesome with Webpack](#11-using-fontawesome-with-webpack)
  - [1. Using FontAwesome with Webpack](#1-using-fontawesome-with-webpack)
- [12. Github Repository](#12-github-repository)
  - [1. How To Use Github Repository](#1-how-to-use-github-repository)
  - [1.1 Link to the Github repository.html](#11-link-to-the-github-repositoryhtml)
- [13. Using ESLint](#13-using-eslint)
  - [1. Configuring ESLint](#1-configuring-eslint)
- [14. Summary](#14-summary)
  - [1. Summary](#1-summary)
  - [2. Bonus Lecture.html](#2-bonus-lecturehtml)


## Resources


https://www.udemy.com/course/webpack-from-beginner-to-advanced/

https://github.com/vp-online-courses/webpack-tutorial


![image-20200418213853538](./assets/image-20200418213853538.png)


```
C:\Users\phuong\AppData\Local\Programs\Python\Python37\python.exe D:/Source/Source_All/python/Test/readfile.py
```



## 1. Introduction
### 1. Introduction
### 2. What you need for this course
## 2. Initial Setup and Integrating Webpack
### 1. Why Do We Need Webpack

C?? nhi???u file js 

### 2. Setting Up Our Application

create file index.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <script src="src/hello-world.js"></script>
    <script src="src/index.js"></script>
    <title>Document</title>
  </head>
  <body></body>
</html>

```

src/index.js

```js
hello();
```

src/hello-world.js

```js
function hello() {
    console.log("hello");
}
```



### 3. Install Webpack And Integrate It With NPM
https://github.com/vp-online-courses/webpack-tutorial/tree/5-install-webpack-end


```shell
npm init -y

npm install --save-dev webpack webpack-cli
```

### Custom webpack configuration
Can Preview

https://github.com/vp-online-courses/webpack-tutorial/blob/8-custom-webpack-configuration-end/webpack.config.js

Add new file to Custom webpack configuration
![](assets/Pasted%20image%2020221002221749.png)
![](assets/Pasted%20image%2020221002221804.png)

**project**

```diff
  webpack-demo
  |- package.json
+ |- webpack.config.js
  |- /dist
    |- index.html
  |- /src
    |- index.js
```

**webpack.config.js**

```javascript
const path = require('path');

module.exports = {
  entry: './src/index.js',
  output: {
    filename: 'bundle.js',
    path: path.resolve(__dirname, 'dist'),
  },
};
```

![](assets/Pasted%20image%2020221002221847.png)

package.json

```js
 "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "build": "webpack"
  },
```

### 4. Small Note about Github Repository.html

Hi guys and girls,

I hope you are enjoying the course so far!

I just want to let you know that there is a [Github Repository](https://github.com/vp-online-courses/webpack-tutorial) containing all the code for this course. If you have any issues with the code, it will help you to resolve those issues and continue with the course.

I am explaining how you can use the Github Repository in **Section 12**.

If you have any questions regarding the course, please feel free to write me via Q&A section and I will do my best to help you!

https://github.com/vp-online-courses/webpack-tutorial

### 4.1 Github Repository.html

https://github.com/vp-online-courses/webpack-tutorial

**NOTE**: l???i error Uncaught SyntaxError: Invalid or unexpected token when run webpack

I fixed the problem by adding the meta tag `` to my index.html and rebuilding.

### 5. Integrating Webpack Into Our JS Application
Can preview

hello-world.js

```js
function hello() {
  console.log("hello");
}

export default hello;

```

index.js

```js
import hello from "./hello-world";

hello();

```

![](assets/Pasted%20image%2020221002221238.png)
![](assets/Pasted%20image%2020221002221422.png)

index.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
        <script src="./dist/bundle.js"></script>
    </body>
</html>


```

`npm run build`

NOTE: l??u ?? ?????n th??? t??? ?????t th??? script

## Asset modules
Preview
![](assets/Pasted%20image%2020221002222404.png)
Resources: large files
inline: small file like svg
asset: general files
source: bundle

### Handle images
https://github.com/vp-online-courses/webpack-tutorial/tree/10-handling-images-with-webpack-end

add-image.js 
```js
import Kiwi from './kiwi.jpg';

function addImage() {
    const img = document.createElement('img');
    img.alt = 'Kiwi';
    img.width = 300;
    img.src = Kiwi;
    const body = document.querySelector('body');
    body.appendChild(img);
}

export default addImage;
```

index.js
```js
import helloWorld from './hello-world.js';
import addImage from './add-image.js';

helloWorld();
addImage();
```

webpack.config.json
```js
const path = require('path');

module.exports = {
    entry: './src/index.js',
    output: {
        filename: 'bundle.js',
        path: path.resolve(__dirname, './dist')
    },
    mode: 'none',
    module: {
        rules: [
            {
                test: /\.(png|jpg)$/,
                type: 'asset/resource'
            }
        ]
    }
};

```

Another example

![](assets/Pasted%20image%2020221002223219.png)
delete the 1st rule
npm run build

![](assets/Pasted%20image%2020221002223331.png)

### publicPath
The??[`publicPath`](https://webpack.js.org/configuration/output/#outputpublicpath)??configuration option can be quite useful in a variety of scenarios. It allows you to specify the base path for all the assets within your application.


https://github.com/vp-online-courses/webpack-tutorial/compare/11-public-path-begin...11-public-path-end

```js
    entry: './src/index.js',
    output: {
        filename: 'bundle.js',
        path: path.resolve(__dirname, './dist'),
        publicPath: 'dist/'
    },
    mode: 'none',
    module: {
```

Open live server
http://127.0.0.1:5500/dist/
Now u can see the image
![](assets/Pasted%20image%2020221002224238.png)


### Asset/inline Module Type

```javascript
const path = require('path');

module.exports = {
    entry: './src/index.js',
    output: {
        filename: 'bundle.js',
        path: path.resolve(__dirname, './dist'),
        publicPath: 'dist/'
    },
    mode: 'none',
    module: {
        rules: [
            {
                test: /\.(png|jpg)$/,
                type: 'asset/inline'
            }
        ]
    }
};

```

### General Asset Type

```javascript
const path = require('path');

module.exports = {
    entry: './src/index.js',
    output: {
        filename: 'bundle.js',
        path: path.resolve(__dirname, './dist'),
        publicPath: 'dist/'
    },
    mode: 'none',
    module: {
        rules: [
            {
                test: /\.(png|jpg)$/,
                type: 'asset',
                parser: {
                    dataUrlCondition: {
                        maxSize: 3 * 1024
                    }
                }
            }
        ]
    }
};


```

### Asset/source Module Type

Add altText.txt

```javascript
import Kiwi from './kiwi.jpg';
import altText from './altText.txt';

function addImage() {
    // Inside this function I will create an img dom element, specify an alt , width , and src properties.
    const img = document.createElement('img');
    img.alt = altText;
    img.width = 300;
    img.src = Kiwi;
    const body = document.querySelector('body');
    body.appendChild(img);
}

export default addImage;
```

webpack

```javascript
const path = require('path');

module.exports = {
    entry: './src/index.js',
    output: {
        filename: 'bundle.js',
        path: path.resolve(__dirname, './dist'),
        publicPath: 'dist/'
    },
    mode: 'none',
    module: {
        rules: [
            {
                test: /\.(png|jpg)$/,
                type: 'asset',
                parser: {
                    dataUrlCondition: {
                        maxSize: 3 * 1024
                    }
                }
            },
            {
                test: /\.txt/,
                type: 'asset/source'
            }
        ]
    }
};

```


## 3. Loaders
### 1. What Is Webpack Loader
### 2. Handling Images With Webpack

add-images.js

```js
import Kiwi from "./kiwi.jpg";

function addImage() {
  const img = document.createElement("img");
  img.src = Kiwi;
  img.alt = "Kiwi";
  img.width = 300;

  const bodyDomElement = document.querySelector("body");
  bodyDomElement.appendChild(img);
}

export default addImage;

```

add in index.js

webpack-config.js

```js
const path = require("path");

module.exports = {
  entry: "./src/index.js",
  output: {
    filename: "bundle.js",
    path: path.resolve(__dirname, "dist"),
  },
  mode: "none",
  module: {
    rules: [
      {
        test: /\.(png|jpg)$/,
        use: ["file-loader"],
      },
    ],
  },
};

```

npm install --save-dev file-loader

npm run build

### 3. Handling Images With Webpack. How To Use publicPath

N???u ????? file index.html ngo??i th?? m???c dist th?? s??? b??? l???i n??n ch??? ra publicPath

![image-20200419094639812](./assets/image-20200419094639812.png)  

```js
const path = require("path");

module.exports = {
  entry: "./src/index.js",
  output: {
    filename: "bundle.js",
    path: path.resolve(__dirname, "dist"),
    publicPath: "dist/", // add sau n??y thay b???ng https://..
  },
  mode: "none",
  module: {
    rules: [
      {
        test: /\.css$/,
        use: ["style-loader", "css-loader"],
      },
      {
        test: /\.(png|svg|jpg|gif)$/,
        use: ["file-loader"],
      },
    ],
  },
};

```



### 4. Handling CSS With Webpack

```js
const path = require("path");

module.exports = {
  entry: "./src/index.js",
  output: {
    filename: "bundle.js",
    path: path.resolve(__dirname, "dist"),
    publicPath: "dist/",
  },
  mode: "none",
  module: {
    rules: [
      {
        test: /\.(png|svg|jpg|gif)$/,
        use: ["file-loader"],
      },
        // add
      {
        test: /\.css$/,
        use: ["style-loader", "css-loader"],
      },
      {
        test: /\.scss$/,
        use: ["style-loader", "css-loader", "sass-loader"],
      },
    ],
  },
};

```

npm install --save-dev sass-loader node-sass style-loader css-loader

*hello-world-button.js*

```js
// import './hello-world-button.scss';
import "./hello-world.css";

class HelloWorldButton {
  //   buttonCssClass = "hello-world-button";

  render() {
    const button = document.createElement("button");
    const br = document.createElement("br");

    const body = document.querySelector("body");
    button.innerHTML = "Hello world";
    button.onclick = function () {
      const p = document.createElement("p");
      p.innerHTML = "Hello world";
      p.classList.add("hello-world-text");
      body.appendChild(p);
    };
    button.classList.add("hello-world-button");
    body.appendChild(br);

    body.appendChild(button);
  }
}

export default HelloWorldButton;

```

hello-world.css

```css
.hello-world-button {
  font-size: 20px;
  padding: 7px 15px;
  background: green;
  color: white;
  outline: none;
}

.hello-world-text {
  color: red;
  font-weight: bold;
}

```

![image-20200419100716059](./assets/image-20200419100716059.png)

### 5. Handling SASS

B??? comment ????? test

hello-world-button.scss

````scss
$font-size: 20px;
$button-background-color: green;
$button-font-color: white;
$text-font-color: red;

.hello-world-button {
    font-size: $font-size;
    padding: 7px 15px;
    background: $button-background-color;
    color: $button-font-color;
    outline: none;
}

.hello-world-text {
    color: $text-font-color;
    font-weight: bold;
}

````



### 6. Using Latest JavaScript Features With Babel 7

hello-world-button.js

```js

class HelloWorldButton {
    // add props
    buttonCssClass = 'hello-world-button';

```

webpack.config.js

```js
const path = require("path");

module.exports = {
  entry: "./src/index.js",
  output: {
    filename: "bundle.js",
    path: path.resolve(__dirname, "dist"),
    publicPath: "dist/",
  },
  mode: "none",
  module: {
    rules: [
      {
        test: /\.(png|svg|jpg|gif)$/,
        use: ["file-loader"],
      },
      {
        test: /\.css$/,
        use: ["style-loader", "css-loader"],
      },
      {
        test: /\.scss$/,
        use: ["style-loader", "css-loader", "sass-loader"],
      },
        // add
      {
        test: /\.js$/,
        exclude: /node_modules/,
        use: {
          loader: "babel-loader",
          options: {
            presets: ["@babel/env"],
            plugins: ["transform-class-properties"],
          },
        },
      },
    ],
  },
};

```

`npm install @babel/core babel-loader @babel/preset-env babel-plugin-transform-class-properties --save-dev`



## 4. Plugins
### 1. What Is Webpack Plugin

![image-20200419102310344](./assets/image-20200419102310344.png)

### 2. Minification Of The Resulting Webpack Bundle

https://webpack.js.org/plugins/terser-webpack-plugin/

```shell
$ npm install terser-webpack-plugin --save-dev
```

L??m nh??? ??i file bundle



### 3. Extracting CSS Into a Separate Bundle With mini-css-extract-plugin, Part 1

https://webpack.js.org/plugins/mini-css-extract-plugin/

To begin, you'll need to install `mini-css-extract-plugin`:

```bash
npm install --save-dev mini-css-extract-plugin
```

```js
const path = require("path");
const TerserPlugin = require("terser-webpack-plugin");
const MiniCssExtractPlugin = require('mini-css-extract-plugin');


module.exports = {
  entry: "./src/index.js",
  output: {
    filename: "bundle.js",
    path: path.resolve(__dirname, "dist"),
    publicPath: "dist/",
  },
  mode: "none",
  module: {
    rules: [
      {
        test: /\.(png|svg|jpg|gif)$/,
        use: ["file-loader"],
      },
      {
        test: /\.css$/,
          // add
        use: [MiniCssExtractPlugin.loader, "css-loader"],
      },
      {
        test: /\.scss$/,
        use: [MiniCssExtractPlugin.loader, "css-loader", "sass-loader"],
      },
      {
        test: /\.js$/,
        exclude: /node_modules/,
        use: {
          loader: "babel-loader",
          options: {
            presets: ["@babel/env"],
            plugins: ["transform-class-properties"],
          },
        },
      },
    ],
  },
    // add
  plugins: [
    new TerserPlugin(),
    new MiniCssExtractPlugin({
      // Options similar to the same options in webpackOptions.output
      // both options are optional
      filename: "styles.css",
    }),
  ],
};


```

index.html add link tag

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="./dist/styles.css" />
    <title>Document</title>
  </head>
  <body>
    <script src="./dist/bundle.js"></script>
  </body>
</html>

```



### 4. Extracting CSS Into a Separate Bundle, Part 2

Th??m heading

### 5. Browser Caching

As you might know, every time your browser loads a website, it downloads all the assets required by this Website. Each Website is different.
However most of them require some javascript and css in order to work properly.
and some Websites require lots of JavaScript. 
Each time the user reloads the page, their browser downloads all those files from the Internet.

With slow internet connection 
Each time they go to a new page they need to wait several minutes until the page is ready.

And it's called browser caching. 
If the file didn't change between the page reloads, your browser can save it in a specific place. This place is called cache.
When you open this page again browser won't download this file again.
It will take this file from cache.
This technique helps to save lots of time and traffic.

What if you fixed a bug on your Website and your javascript file has been changed? If the browser always  takes this file from cache your customers will never get the new version.
Therefore we need a mechanism for updating the cache.
One of the most popular approaches is creating a new file with the new name
each time you make a change. Browsers remember files by name.
Therefore if the name changes browsers will download the new version.
Well it doesn't mean that we need to change the filename manually every time we change our code.
We can do this automatically.
md5 ?????t t??n file trong d???u []

```js

  output: {
    filename: "bundle.[contenthash].js", // add

        ...
    
    
  plugins: [
    new TerserPlugin(),
    new MiniCssExtractPlugin({
      // Options similar to the same options in webpackOptions.output
      // both options are optional
      filename: "styles.[contenthash].css", // add
    }),
  ],
```



### 6. How To Clean Dist Folder Before Generating New Bundles

```
npm install --save-dev clean-webpack-plugin
```

https://www.npmjs.com/package/clean-webpack-plugin

```js

const { CleanWebpackPlugin } = require("clean-webpack-plugin");

...

  plugins: [
    new CleanWebpackPlugin(),
    new TerserPlugin(),
    new MiniCssExtractPlugin({
      // Options similar to the same options in webpackOptions.output
      // both options are optional
      filename: "styles.[contenthash].css",
    }),
  ],
```

X??a h???t file tring dist/

????? x??a t???t c??? file trong build folder

```js

  plugins: [
    new CleanWebpackPlugin({
      cleanOnceBeforeBuildPatterns: [
        "**/*",
        path.join(process.cwd(), "build/**/*"),
      ],
    }),
    new TerserPlugin(),
    new MiniCssExtractPlugin({
      // Options similar to the same options in webpackOptions.output
      // both options are optional
      filename: "styles.[contenthash].css",
    }),
  ],
```

### 7. Generating HTML Files Automatically During Webpack Build Process

L??c load l???i file index.html s??? l???i v?? include kh??ng bao g???m md5

https://webpack.js.org/plugins/html-webpack-plugin/

```bash
npm install --save-dev html-webpack-plugin
```

N???u c?? publicPath th?? file index.html s??? t??? ?????ng th??m v??o link do ???? n??n x??a ??i ????? r???ng

Sau ???? x??a file html ??? ngo??i ??i

```js
const path = require("path");
const TerserPlugin = require("terser-webpack-plugin");
const MiniCssExtractPlugin = require("mini-css-extract-plugin");
const { CleanWebpackPlugin } = require("clean-webpack-plugin");
const HtmlWebpackPlugin = require("html-webpack-plugin");

module.exports = {
  entry: "./src/index.js",
  output: {
    filename: "bundle.[contenthash].js",
    path: path.resolve(__dirname, "dist"),
    publicPath: "",
  },
  mode: "none",
  module: {
    rules: [
      {
        test: /\.(png|svg|jpg|gif)$/,
        use: ["file-loader"],
      },
      {
        test: /\.css$/,
        use: [MiniCssExtractPlugin.loader, "css-loader"],
      },
      {
        test: /\.scss$/,
        use: [MiniCssExtractPlugin.loader, "css-loader", "sass-loader"],
      },
      {
        test: /\.js$/,
        exclude: /node_modules/,
        use: {
          loader: "babel-loader",
          options: {
            presets: ["@babel/env"],
            plugins: ["transform-class-properties"],
          },
        },
      },
    ],
  },
  plugins: [
    new CleanWebpackPlugin({
      cleanOnceBeforeBuildPatterns: [
        "**/*",
        path.join(process.cwd(), "build/**/*"),
      ],
    }),
    new TerserPlugin(),
    new MiniCssExtractPlugin({
      // Options similar to the same options in webpackOptions.output
      // both options are optional
      filename: "styles.[contenthash].css",
    }),
    new HtmlWebpackPlugin(), // add
  ],
};

```



### 8. Customizing Generated HTML Files

https://www.npmjs.com/package/html-webpack-plugin

```js
new HtmlWebpackPlugin({
      filename: "sub/hello-world.html",
      title: "Hello world",
      meta: {
        description: "description Hello world",
      },
    }),
```

gen ra file html trong th?? m???c sub

### 9. Integration with Handlebars

https://github.com/jantimon/html-webpack-plugin

https://github.com/jantimon/html-webpack-plugin/blob/master/docs/template-option.md

```js
{
                test: /\.hbs$/,
                use: [
                    'handlebars-loader'
                ]
            }

....


new HtmlWebpackPlugin({
      title: "Hello world",
      description: "description Hello world",
      template: "src/page-template.hbs",
    }),
```

src/page-template.hbs

```js
<!doctype html>

<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="{{htmlWebpackPlugin.options.description}}">
    <title>{{htmlWebpackPlugin.options.title}}</title>
</head>
<body>

</body>
</html>

```

`npm install handlebars-loader --save-dev`

`npm install --save handlebars`



### 10. More Webpack Plugins

### 

## 5. Production vs Development Builds
### 1. Introduction
### 2. Mode

index.js

```js

// mode
if (process.env.NODE_ENV === "production") {
  console.log("production mode");
} else if (process.env.NODE_ENV === "development") {
  console.log("developent mode");
}

// check file error position
// helloWorldButton.acb();
```

S???a mode in webpack

### 3. Managing Webpack Config for Production and Development Use Cases

Tach ra 2 file

??? production mode x??a plugin terser

webpack.dev.config

```js
const path = require("path");
const { CleanWebpackPlugin } = require("clean-webpack-plugin");
const HtmlWebpackPlugin = require("html-webpack-plugin");

module.exports = {
  entry: "./src/index.js",
  output: {
    filename: "bundle.js", // add
    path: path.resolve(__dirname, "dist"),
    publicPath: "",
  },
  mode: "development",
  module: {
    rules: [
      {
        test: /\.(png|svg|jpg|gif)$/,
        use: ["file-loader"],
      },
      {
        test: /\.css$/,
        use: ["style-loader", "css-loader"], // fix
      },
      {
        test: /\.scss$/,
        use: ["style-loader", "css-loader", "sass-loader"],
      },
      {
        test: /\.js$/,
        exclude: /node_modules/,
        use: {
          loader: "babel-loader",
          options: {
            presets: ["@babel/env"],
            plugins: ["transform-class-properties"],
          },
        },
      },
      {
        test: /\.hbs$/,
        use: ["handlebars-loader"],
      },
    ],
  },
  plugins: [
    new CleanWebpackPlugin({
      cleanOnceBeforeBuildPatterns: [
        "**/*",
        path.join(process.cwd(), "build/**/*"),
      ],
    }),
      // remove 2
    new HtmlWebpackPlugin({
      title: "Hello world",
      description: "description Hello world",
      template: "src/page-template.hbs",
    }),
  ],
};

```

webpack.production.config

```js
const path = require("path");
const MiniCssExtractPlugin = require("mini-css-extract-plugin");
const { CleanWebpackPlugin } = require("clean-webpack-plugin");
const HtmlWebpackPlugin = require("html-webpack-plugin");

module.exports = {
  entry: "./src/index.js",
  output: {
    filename: "bundle.[contenthash].js",
    path: path.resolve(__dirname, "dist"),
    publicPath: "",
  },
  mode: "production",
  module: {
    rules: [
      {
        test: /\.(png|svg|jpg|gif)$/,
        use: ["file-loader"],
      },
      {
        test: /\.css$/,
        use: [MiniCssExtractPlugin.loader, "css-loader"],
      },
      {
        test: /\.scss$/,
        use: [MiniCssExtractPlugin.loader, "css-loader", "sass-loader"],
      },
      {
        test: /\.js$/,
        exclude: /node_modules/,
        use: {
          loader: "babel-loader",
          options: {
            presets: ["@babel/env"],
            plugins: ["transform-class-properties"],
          },
        },
      },
      {
        test: /\.hbs$/,
        use: ["handlebars-loader"],
      },
    ],
  },
  plugins: [
    new CleanWebpackPlugin({
      cleanOnceBeforeBuildPatterns: [
        "**/*",
        path.join(process.cwd(), "build/**/*"),
      ],
    }),
    new MiniCssExtractPlugin({
      // Options similar to the same options in webpackOptions.output
      // both options are optional
      filename: "styles.[contenthash].css",
    }),
    new HtmlWebpackPlugin({
      title: "Hello world",
      description: "description Hello world",
      template: "src/page-template.hbs",
    }),
  ],
};

```

package.json

```js

  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "build": "webpack --config webpack.production.config.js",
    "dev": "webpack --config webpack.dev.config.js",
    "start": "node src/server.js"
  },
```

??? mode dev d??? track error

![image-20200419155639230](./assets/image-20200419155639230.png)

### 4. Faster Development with webpack dev server

```bash
npm install webpack-dev-server --save-dev
```

webpack-dev-config.js

```js
const path = require("path");
const { CleanWebpackPlugin } = require("clean-webpack-plugin");
const HtmlWebpackPlugin = require("html-webpack-plugin");

module.exports = {
  entry: "./src/index.js",
  output: {
    filename: "bundle.js",
    path: path.resolve(__dirname, "dist"),
    publicPath: "",
  },
    // add
  devServer: {
    contentBase: path.resolve(__dirname, "./dist"),
    index: "index.html",
    port: 9000,
  },
  mode: "development",
  module: {
    rules: [
      {
        test: /\.(png|svg|jpg|gif)$/,
        use: ["file-loader"],
      },
      {
        test: /\.css$/,
        use: ["style-loader", "css-loader"],
      },
      {
        test: /\.scss$/,
        use: ["style-loader", "css-loader", "sass-loader"],
      },
      {
        test: /\.js$/,
        exclude: /node_modules/,
        use: {
          loader: "babel-loader",
          options: {
            presets: ["@babel/env"],
            plugins: ["transform-class-properties"],
          },
        },
      },
      {
        test: /\.hbs$/,
        use: ["handlebars-loader"],
      },
    ],
  },
  plugins: [
    new CleanWebpackPlugin({
      cleanOnceBeforeBuildPatterns: [
        "**/*",
        path.join(process.cwd(), "build/**/*"),
      ],
    }),
    new HtmlWebpackPlugin({
      title: "Hello world",
      description: "description Hello world",
      template: "src/page-template.hbs",
    }),
  ],
};

```

package.json

```js

  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "build": "webpack --config webpack.production.config.js",
    "dev": "webpack-dev-server --config webpack.dev.config.js --hot", // add
    "start": "node src/server.js"
  },
```

npm run dev :  s???a s??? load l???i on browser

### 5. Cleaning Up A Bit

## 6. Multiple Page Applications
### 1. Introduction
### 2. Creating KiwiImage Component

kiwi-images.js

```js
import Kiwi from './kiwi.jpg';
import './kiwi-image.scss';

class KiwiImage {
    render() {
        const img = document.createElement('img');
        img.src = Kiwi;
        img.alt = 'Kiwi';
        img.classList.add('kiwi-image');

        const bodyDomElement = document.querySelector('body');
        bodyDomElement.appendChild(img);
    }
}

export default KiwiImage;

```

kiwi-images.scss

```scss
.kiwi-image {
    display: block;
    width: 400px;
    height: auto;
}


```

### 3. Code Splitting in Webpack Multiple JS and CSS Bundles

src/kiwi.js

```js
import Heading from './components/heading/heading.js';
import KiwiImage from './components/kiwi-image/kiwi-image.js';

const heading = new Heading();
heading.render('kiwi');
const kiwiImage = new KiwiImage();
kiwiImage.render();

```

webpack.production.config.js

```js
const path = require("path");
const MiniCssExtractPlugin = require("mini-css-extract-plugin");
const { CleanWebpackPlugin } = require("clean-webpack-plugin");
const HtmlWebpackPlugin = require("html-webpack-plugin");

module.exports = {
  // add
  entry: {
    "hello-world": "./src/hello-world.js",
    kiwi: "./src/kiwi.js",
  },
  output: {
    filename: "[name].[contenthash].js", // fix
    path: path.resolve(__dirname, "dist"),
    publicPath: "",
  },
  mode: "production",
  module: {
    rules: [
      {
        test: /\.(png|svg|jpg|gif)$/,
        use: ["file-loader"],
      },
      {
        test: /\.css$/,
        use: [MiniCssExtractPlugin.loader, "css-loader"],
      },
      {
        test: /\.scss$/,
        use: [MiniCssExtractPlugin.loader, "css-loader", "sass-loader"],
      },
      {
        test: /\.js$/,
        exclude: /node_modules/,
        use: {
          loader: "babel-loader",
          options: {
            presets: ["@babel/env"],
            plugins: ["transform-class-properties"],
          },
        },
      },
      {
        test: /\.hbs$/,
        use: ["handlebars-loader"],
      },
    ],
  },
  plugins: [
    new CleanWebpackPlugin({
      cleanOnceBeforeBuildPatterns: [
        "**/*",
        path.join(process.cwd(), "build/**/*"),
      ],
    }),
    new MiniCssExtractPlugin({
      // Options similar to the same options in webpackOptions.output
      // both options are optional
      filename: "[name].[contenthash].css",  // fix
    }),
    new HtmlWebpackPlugin({
      title: "Hello world",
      description: "description Hello world",
      template: "src/page-template.hbs",
    }),
  ],
};

```

S???a name v?? entry cho dev

`npm run build`

### 4. How To Generate Multiple HTML Files

file index.html ???????c sinh ra c?? d???ng

```js
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <meta name="description" content="description Hello world" />
    <title>Hello world</title>
    <link href="kiwi.18009c082a7520ea9379.css" rel="stylesheet" />
  </head>
  <body>
    <script src="hello-world.13c8eb137cbb4147c189.js"></script>
    <script src="kiwi.93c2223e1e05e13a7fa9.js"></script>
  </body>
</html>

```

production

```js
new HtmlWebpackPlugin({
            filename: 'hello-world.html',
            chunks: ['hello-world'],
            title: 'Hello world',
            description: 'Hello world',
            template: 'src/page-template.hbs'
        }),
        new HtmlWebpackPlugin({
            filename: 'kiwi.html',
            chunks: ['kiwi'],
            title: 'Kiwi',
            description: 'Kiwi',
            template: 'src/page-template.hbs'
        })
// chunk c?? t??n tr??ng v???i entry
```



### 5. Extracting Common Dependencies While Code Splitting

truy???n name v??o header

kiwi.js

```js
import Heading from "./components/heading/heading.js";
import KiwiImage from "./components/kiwi-image/kiwi-image.js";
import _ from "lodash"; // add

const heading = new Heading();
heading.render(_.upperFirst("kiwi"));
const kiwiImage = new KiwiImage();
kiwiImage.render();

```

Khi build ra t???i 70kb qu?? l???n v?? lodash, m???i l???n l???i download v??? => slow

prodcution

```js

  mode: "production",
  optimization: {
    splitChunks: {
      chunks: "all",
    },
  },
      
      
    // add chunk
  
    new HtmlWebpackPlugin({
      filename: "hello-world.html",
      chunks: ["hello-world", "vendors~hello-world~kiwi"],
      title: "Hello world",
      description: "Hello world",
      template: "src/page-template.hbs",
    }),
    new HtmlWebpackPlugin({
      filename: "kiwi.html",
      chunks: ["kiwi", "vendors~hello-world~kiwi"],
      title: "Kiwi",
      description: "Kiwi",
      template: "src/page-template.hbs",
    }),
```


```
It is called optimization.
It is an object and inside it we can specify another option which is called splitChunks.
And inside we need to specify yet another option which is called chunks, and here specify the value "all".

And we have now third javascript bundle 
which is called vendors~hello-world~kiwi.<something>.js which consumes around 70 kilobytes. So in this bundle
we have lodash.
This third bundle will be cached separately and now our users don't need to download it when we change something in kiwi.js
or hello-world.js. Since we have a new bundle, how webpack knows where to include it?

Will all html pages include it by default? 
The answer is we should specifically tell webpack to include it for every html page that needs it.
In our case both our pages need this bundle.

So now let's go back to our editor to our webpack configuration and scroll down to the HtmlWebpackPlugin.

And here remember we included chunks.
So now every our html page would need two chunks instead of one
And the second chunk would be this common chunk, common bundle, which includes lodash library. 

Which is called
vendors~hello-world~kiwi.
```


### 6. Setting Custom Options for Code Splitting

npm install react --save

kiwi.js

```js
import Heading from "./components/heading/heading.js";
import KiwiImage from "./components/kiwi-image/kiwi-image.js";
import React from "react";
// import _ from "lodash";

const heading = new Heading();
// heading.render(_.upperFirst("kiwi"));
heading.render("kiwi");
const kiwiImage = new KiwiImage();
kiwiImage.render();

```

webpack.production.config

```js

    mode: 'production',
    optimization: {
        splitChunks: {
            chunks: 'all',
            minSize: 10000,
            automaticNameDelimiter: '_'
        }
    },
```

![image-20200419174143284](./assets/image-20200419174143284.png)  

V?? lodash > 30kb react th?? nh??? h??n n??n k ho???t ?????ng

![image-20200419174542272](./assets/image-20200419174542272.png)

### 7. How To Setup Development Environment For Multiple Page Application

webpack.dev.config

```js
const path = require("path");
const { CleanWebpackPlugin } = require("clean-webpack-plugin");
const HtmlWebpackPlugin = require("html-webpack-plugin");

module.exports = {
  entry: {
    "hello-world": "./src/hello-world.js",
    kiwi: "./src/kiwi.js",
  },
  output: {
    filename: "[name].bundle.js",
    path: path.resolve(__dirname, "dist"),
    publicPath: "",
  },
  devServer: {
    contentBase: path.resolve(__dirname, "./dist"),
    index: "index.html",
    port: 9000,
  },
  mode: "development",
  module: {
    rules: [
      {
        test: /\.(png|svg|jpg|gif)$/,
        use: ["file-loader"],
      },
      {
        test: /\.css$/,
        use: ["style-loader", "css-loader"],
      },
      {
        test: /\.scss$/,
        use: ["style-loader", "css-loader", "sass-loader"],
      },
      {
        test: /\.js$/,
        exclude: /node_modules/,
        use: {
          loader: "babel-loader",
          options: {
            presets: ["@babel/env"],
            plugins: ["transform-class-properties"],
          },
        },
      },
      {
        test: /\.hbs$/,
        use: ["handlebars-loader"],
      },
    ],
  },
  plugins: [
    new CleanWebpackPlugin({
      cleanOnceBeforeBuildPatterns: [
        "**/*",
        path.join(process.cwd(), "build/**/*"),
      ],
    }),
    new HtmlWebpackPlugin({
      title: "Hello world",
      description: "description Hello world",
      template: "src/page-template.hbs",
    }),
  ],
};

```

http://localhost:9000/kiwi.html

## 7. Webpack Integration With Node And Express
### 1. Introduction
### 2. Getting Code for Single Page Application.html

As I said in the previous video, first we will integrate Express framework into a Single Page Application. We will use code from Section 5 as a starting point. You can get this code from the [Github repository](https://github.com/vp-online-courses/webpack-tutorial). Just follow 3 easy steps:

\1. First, you need to clone this repository to your computer.

```bash
git clone https://github.com/vp-online-courses/webpack-tutorial.git
cd webpack-tutorial
```

\2. Then checkout the branch `integrating-express-js-into-a-single-page-application`.

```shell
git checkout -b integrating-express-js-into-a-single-page-application remotes/origin/integrating-express-js-into-a-single-page-application
```

\3. Finally, don't forget to reinstall project dependencies after switching to the new branch.

```bash
rm -rf node_modules
npm install
```

At this point you have all the files you need in order to integrate Express framework into a Single Page Application.

### 3. Integrating Express Into Our Application

npm install --save express

package.json

```js
"start": "node src/server.js"
```

src/server.js

```js
const express = require("express");
const app = express();

app.get("/", function (req, res) {
  res.send("Some dummy content");
});

app.listen(3000, function () {
  console.log("Application is running on http://localhost:3000");
});

```

npm start

### 4. Serving HTML Pages via Express

server.js

```js
const express = require('express');
const app = express();
const path = require('path');
const fs = require('fs');


app.get("/", function (req, res) {
  const pathToHtmlFile = path.resolve(__dirname, "../dist/index.html");
  const contentFromHtmlFile = fs.readFileSync(pathToHtmlFile, "utf-8");
  res.send(contentFromHtmlFile);
});

// ph???n sau
app.use('/static', express.static(path.resolve(__dirname, '../dist')));

app.listen(3000, function () {
    console.log('Application is running on http://localhost:3000');
});

```

npm run build

npm start

![image-20200419211606404](./assets/image-20200419211606404.png)  

![image-20200419211656513](./assets/image-20200419211656513.png)

N???u l?? static file n?? s??? t??m trong static folder

### 5. Handling JS and CSS via Express

prodcution

```js

module.exports = {
  entry: "./src/index.js",
  output: {
    filename: "bundle.[contenthash].js",
    path: path.resolve(__dirname, "./dist"),
    publicPath: "/static/",  // add thay v?? add th??? c??ng t???ng c??i
  },
```



### 6. Getting Code for Multiple Page Application.html

In the next video we will integrate Express framework into a Multiple Page Application. We will use code from Section 6 as a starting point. You can get this code from the Github repository. Just follow 3 easy steps:

\1. First, you need to clone [this repository](https://github.com/vp-online-courses/webpack-tutorial) to your computer.

```
git clone https://github.com/vp-online-courses/webpack-tutorial.git
cd webpack-tutorial
```

\2. Then checkout the branch `integrating-express-js-into-a-multiple-page-application`.

```
git checkout -b integrating-express-js-into-a-multiple-page-application remotes/origin/integrating-express-js-into-a-multiple-page-application
```

\3. Finally, don't forget to reinstall project dependencies after switching to the new branch.

```
rm -rf node_modules
npm install
```

At this point you have all the files you need in order to integrate Express framework into a Multiple Page Application.

### 7. Integrating Express.js Into A Multiple Page Application

server.js

```js
const express = require('express');
const app = express();
const path = require('path');
const fs = require('fs');

app.get('/hello-world/', function (req, res) {
    const pathToHtmlFile = path.resolve(__dirname, '../dist/hello-world.html');
    const contentFromHtmlFile = fs.readFileSync(pathToHtmlFile, 'utf-8');
    res.send(contentFromHtmlFile);
});
app.get('/kiwi/', function (req, res) {
    const pathToHtmlFile = path.resolve(__dirname, '../dist/kiwi.html');
    const contentFromHtmlFile = fs.readFileSync(pathToHtmlFile, 'utf-8');
    res.send(contentFromHtmlFile);
});

app.use('/static', express.static(path.resolve(__dirname, '../dist')));

app.listen(3000, function () {
    console.log('Application is running on http://localhost:3000');
});

```

```shell
npm install
npm run build
npm start
```



## 8. Integration with jQuery
### 1. Getting the Source Code.html

In this section (and in the next sections as well) you would need to use [Github repository](https://github.com/vp-online-courses/webpack-tutorial) associated with this course. We'll use the source code from `starting-point-for-use-cases` branch as a starting point.

Let me show you how you can get the source code:

\1. First, you need to clone the Github repository.

```
git clone https://github.com/vp-online-courses/webpack-tutorial.git
cd webpack-tutorial
```

\2. Second, you need to checkout the branch `starting-point-for-use-cases`.

```
git checkout -b starting-point-for-use-cases remotes/origin/starting-point-for-use-cases
```

\3. Finally, you need to install the project dependencies after switching to the new branch.

```
rm -rf node_modules
npm install
```

Now you are ready to start with this section.



P. S. You would need to repeat these steps every time you start one of the following sections:

\1. Integration with jQuery.

\2. Integration with Bootstrap.

\3. Using FontAwesome with Webpack.

\4. Using ESLint.

### 2. Integration with jQuery
## 9. Using Custom Fonts with Webpack
### 1. Using Custom Fonts with Webpack

npm install jquery --save

![image-20200419214121248](./assets/image-20200419214121248.png)  

npm run build

npm start

## 10. Integration with Bootstrap

### 1. Using Bootstrap with Webpack

npm install bootstrap --save

X??i bs 3 bs 4 l???i

https://github.com/twbs/bootstrap/issues/27353

https://webpack.js.org/configuration/externals/

index.js

```js
import "bootstrap";
import "bootstrap/dist/css/boostrap.min.css";
import "./index.scss
```

page-template.hbs

```html
<!doctype html>

<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="{{htmlWebpackPlugin.options.description}}">
    <title>{{htmlWebpackPlugin.options.title}}</title>
</head>
<body>
    <div class="alert alert-primary" role="alert">
        This is a primary alert???check it out!
    </div>

    <div class="dropdown my-dropdown">
        <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            Dropdown button
        </button>
        <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
            <a class="dropdown-item" href="#">Action</a>
            <a class="dropdown-item" href="#">Another action</a>
            <a class="dropdown-item" href="#">Something else here</a>
        </div>
    </div>
</body>
</html>
```

index.scss

```scss
  
.my-dropdown {
    float: right;
    position: relative;
    top: 7px;
    right: 40px;
}
```

npm run build

npm start

### 2. 2nd Method Of Importing CSS From Bootstrap

```js
{
                test: /\.scss$/,
                use: [
                    MiniCssExtractPlugin.loader,
                    'css-loader',
                    {
                        loader: 'postcss-loader',
                        options: {
                            plugins: function () {
                                return [
                                    require('precss'),
                                    require('autoprefixer')
                                ];
                            }
                        }
                    },
                    'sass-loader'
                ]
            },
```



## 11. Using FontAwesome with Webpack

### 1. Using FontAwesome with Webpack

![image-20200419214418991](./assets/image-20200419214418991.png)  

gg: google font open sans

![image-20200419214539769](./assets/image-20200419214539769.png)  

Sau ???? t???i v???

X??a ch??? gi??? l???i 3 c??i:

![image-20200419214709335](./assets/image-20200419214709335.png)  

gg: online font converter r???i ch???n

![image-20200419214813973](./assets/image-20200419214813973.png)  

![image-20200419215228081](./assets/image-20200419215228081.png)  

V??o index.js import "./index.scss" ?????u ti??n

![image-20200419215544660](./assets/image-20200419215544660.png)  

thay cho 2 file r???i run 

```shell
npm install --save-dev file-loader
npm run dev
```





## 12. Github Repository

### 1. How To Use Github Repository

```shell
git branch -a

```

![image-20200419162701151](./assets/image-20200419162701151.png)  

check out qua end

`git reset --hard HEAD`

### 1.1 Link to the Github repository.html

https://github.com/vp-online-courses/webpack-tutorial

## 13. Using ESLint

### 1. Configuring ESLint

npm install --save-dev eslint

package.json

```js
"lint": "eslint ."
```

![image-20200419233358372](./assets/image-20200419233358372.png)

## 14. Summary

### 1. Summary

### 2. Bonus Lecture.html


