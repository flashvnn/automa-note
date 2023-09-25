## Read/write storage variables

**Define variables**

![automa-storage-variable](images/automa-storage-variable.png)

```js
// Read the storage variables with javascript block
var value = automaRefData('variables', '$$global_links');

// Write the storage variables with javascript block
automaSetVariable('$$global_links', "UPDATED VARIABLES");

console.log(automaRefData('variables', '$$global_links'));
```
