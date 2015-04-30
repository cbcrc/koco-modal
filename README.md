# koco-modal
Modal wrapper when creating a new modal using the [koco generator](https://github.com/cbcrc/generator-koco).

## Installation
```bash
bower install koco-modal
```

## Usage with KOCO

The `koco-modal` component comes with knockout component register function. So, in this case you only have to include this script in the `startup.js` file like so:

```javascript
// startup.js
define([..., 'bower_components/koco-modal/src/koco-modal'], 
  function(...) {
});
```

## Creating a modal

Now that the component is registered, a new html tag named `<modal>` will be available to be used and will initialize a [bootstrap](https://getbootstrap.com) modal.

```html
<modal>
  <h1>My awesome modal title</h1>
  <p>Some cool description...</p>
</modal>
```

## Remarks

This component *does not* register your new modal, it is just a wrapper for the bootstrap html needed to create a modal. You still need to use [modaler](https://github.com/cbcrc/knockout-modaler).
