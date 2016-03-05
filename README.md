# Cesium Webpack Boilerplate #

This project sets a minimal environment for easily getting started with [CesiumJs](https://cesiumjs.org). It uses **webpack** as a build tool and **npm** as a task runner.

## What it does ##
This boilerplate allows you to **experiment quickly** and focus on your project rather than loose time to configure it.

It follows the patterns described in [this tutorial](https://cesiumjs.org/2016/01/26/Cesium-and-Webpack/#using-the-source) to setup a minimal working environment and add some tasks to improve your workflow.

You get a functionnal and distributable cesium application with a unique entry point.

## How to use it ##

```
git clone https://github.com/maxdow/cesiumjs-webpack-boilerplate
cd cesiumjs-webpack-boilerplate
npm install
```

All that you need is installed. Let's start to build and launch a server to see the magic happens.

```
npm run dev
```

Open a browser. The default adress is localhost:8080 ( you can easily customise this inside the package.json file, see [webpack-dev-server documentation](https://webpack.github.io/docs/webpack-dev-server.html) for more options)

Now, take a look at the *src* folder . You will find 2 files :

- **index.html**  the base html with only one div which contain the Cesium viewer widget.
- **app.js**      application main entry point requiring Cesium lib an initialising the viewer.



As a bonus, if you want to make a snapshot release of your app, you can use the npm release task ( `npm run release` ) which will minimize your code thanks to uglify. The complete application will be in the *public* folder

## TODO ##

Add true live-reload
