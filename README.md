# DEPRECATED: Now comes within [koco-modaler](https://github.com/cbcrc/koco-modaler)

# koco-modal
Modal wrapper when creating a new modal using the [koco generator](https://github.com/cbcrc/generator-koco).

## Installation
```bash
bower install koco-modal
```

## Usage with KOCO

The `koco-modal` can be initialized using the [knockout-utilities](https://github.com/cbcrc/knockout-utilities) `registerComponent` function like so:

```javascript
// components.js
...
koUtilities.registerComponent('modal', {
  htmlOnly: true,
  basePath: 'bower_components/koco-modal/src'
});
...
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
