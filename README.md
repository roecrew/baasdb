# baasdb
<p align="middle"><img src="https://farm8.staticflickr.com/7158/6506504319_26600f4d09_b.jpg">
<h3 align="middle">A Micro DB</h3>

## Methods

.create('collection-name', (optional)json) ... returns promise resolve() catch(err)

.fetch('collection-name') ... returns promise resolve(object) catch(err)

.update('collection-name', json) ... returns promise resolve() catch(err)

.destroy('collection-name') ... returns promise resolve() catch(err)

## Example

```
npm install baasdb
```


```js

const baasdb = require('baasdb');

baasdb.create('items');
baasdb.update('items', {a: 1, b: "two", c: [1, 2, 3]});
baasdb.fetch('items').then((obj) => { console.log(obj); });
baasdb.destroy('items');

```
