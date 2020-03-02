 simple react/redux app lifted from scotch.io's tutorial [Getting Started with React and Redux Courses](https://scotch.io/courses/getting-started-with-react-and-redux/introduction)

 Fair warning this course was recorded well over a couple years ago and several of the babel libraries have since been deprecated. Babel has moved from 'babel' packages to [scoped packages](https://docs.npmjs.com/about-scopes). To resolve this the dev dependencies you have to add are in the '@babel/<package>' format

 for this project we used the following installation scripts*

`npm install react react-dom react-redux redux redux-thunk`

`npm install --save-dev @babel/core @babel/preset-env @babel/preset-react babel-loader file-loader react-hot-loader webpack webpack-dev-server`

Additionally with the deprecation es2015 the .babelrc file will be updated as follows:

```
{
    "presets": ["@babel/env", "@babel/react"],
    "plugins": [
        "react-hot-loader/babel"
      ]
  }
```
*credit goes to this [blogpost](http://flummox-engineering.blogspot.com/2018/11/webpack--babel-react-reactjs-pluginpreset-files-are-not-allowed-to-export-objects-only-functions.html)