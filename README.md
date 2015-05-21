# BEM cheat sheet

## BEM tools

Tools that help to do BEM

### $ git clone https://github.com/bem/project-stub.git

Install project stub

### $ sudo npm install bem-cli -g

Install bem-tools globally

### JavaScript

```js
this.getMod(modName)
```
Get mod value

```js
this.getMod(elem, modName)
```
Get element mod value

```js
this.hasMod([elem], modName, modVal)
```
Check whether the block (element) has the modifier.

```js
this.setMod([elem], modName, modVal)
```
Set modificator. **NOTE: This doesn't work:**
```js
this.elem('elemName').setMod(...)
```

```js
this.delMod([elem], modName)
```
Delete modifier.

```js
this.toggleMod([elem], modName, modVal1, modVal2, [condition])
```
Toggle modifiers.
