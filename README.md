**Multiple entry**
```js
module.exports = {
  entry: {
    main: './src/index.js',
    about: './src/about.js',
    contact: './src/contact.js',
  },
  output: {
    filename: '[name].bundle.js',
    path: path.resolve(__dirname, 'dist'),
  },
  optimization: {
    splitChunks: {
      chunks: 'all',
    },
  },
};
```
