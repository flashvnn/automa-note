## Read/write storage variables

**Define storage variables**

![automa-storage-variable](images/automa-storage-variable.png)

```js
// Read the storage variables with javascript block
var value = automaRefData('variables', '$$global_links');

// Write the storage variables with javascript block
automaSetVariable('$$global_links', "UPDATED VARIABLES");

console.log(automaRefData('variables', '$$global_links'));
```

## Access workflow variable

![workflow variable](images/access_workflow_variable.png)

https://docs.automa.site/workflow/expressions.html

**variable in setting block**

```
{{ variables.current_url }}
```

**Get workflow variable in Javascript block**

```js
const value = automaRefData('variables', 'current_url');

console.log("current_url", value);

automaNextBlock()
```

