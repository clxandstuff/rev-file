# rev-file

> Get the revved file path of a file

Reads the file, MD5-hashes it, truncates the hash to [10 characters](https://github.com/sindresorhus/rev-hash), appends it to the filename, and returns the modified path.


## Install

```
$ npm install rev-file
```


## Usage

```js
const revFile = require('rev-file');

revFile('src/unicorn.png').then(filepath => {
	console.log(filepath);
	//=> 'src/unicorn-bb9d8fe615.png'
});
```


## API

### revFile(filepath)

Returns a `Promise` for a revved filepath.

### revFile.sync(filepath)

Returns a revved filepath.


## License

MIT © [Sindre Sorhus](https://sindresorhus.com)
