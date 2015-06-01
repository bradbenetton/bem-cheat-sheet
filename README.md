# BEM cheat sheet

## BEM tools

Tools that help to do BEM

Install project stub

```bash
$ git clone https://github.com/bem/project-stub.git
```

Install bem-tools globally

```bash
$ sudo npm install bem-cli -g
```

### Libraries

BEM Grid

```bash
$ bower install bem-incubator/bem-grid --save
```

BEM Typography

```bash
bower install verybigman/bem-typography --save
```

### JavaScript

Get mod value

```js
this.getMod(modName)
```

Get element mod value

```js
this.getMod(elem, modName)
```

Check whether the block (element) has the modifier.

```js
this.hasMod([elem], modName, modVal)
```
Set modifier.  

```js
this.setMod([elem], modName, modVal)
```

**NOTE: This doesn't work:**

```js
this.elem('elemName').setMod(...)
```

Delete modifier.

```js
this.delMod([elem], modName)
```

Toggle modifiers.

```js
this.toggleMod([elem], modName, modVal1, modVal2, [condition])
```

поиск внутри контекста
```js
this.findBlockInside([elem], block)
```

поиск снаружи контекста
```js
this.findBlockOutside([elem], block)
```

поиск на DOM-узле текущего блока
```js
this.findBlockOn([elem], block)
```
поиск внутри контекста
```js
this.findBlocksInside([elem], block)
```

// поиск снаружи контекста
```js
this.findBlocksOutside([elem], block)
```

// поиск на BEM-узле текущего блока
```js
this.findBlocksOn([elem], block)
```

//кэширующий селектор
```js
this.elem(name, [modName], [modVal])
```

//некэширующий
```js
this.findElem([ctx], name, [modName], [modVal])
```
