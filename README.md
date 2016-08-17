[![Build Status](https://travis-ci.org/willydouhard/expandable-card.svg?branch=master)](https://travis-ci.org/willydouhard/expandable-card)

_[Demo and API docs](https://willydouhard.github.io/expandable-card/components/expandable-card/)_

WARNING: This component is relying on the web animation api. The poly fill is in the component dependencies, so you just have to include it in your index.html file.

Example:

```html
<script src="bower_components/web-animations-js/web-animations-next-lite.min.js"></script>
```

`expandable-card` is a card that can expand (like you see on mobile native apps).

Example:

```html
<expandable-card
  retracted-title="Retracted title"
  retracted-content="Retracted content"
  expanded-title="Expanded title"
  expanded-content="Expanded content">
</expandable-card>
```

Its not possible to think of all the use case for this type of component.
Hence, you should really customize it to fit your needs.
Maybe you want another element of your card to be animated instead of the header while expanding,
or maybe you want to pass an image property for your card.
Don't be afraid to tweak this component as you want.

`expandable-card` by itself is not very useful, because you will probably want
to use more than one. To get multiple `expandable-card` that expands to fit a container
see [expandable-card-container](https://customelements.io/willydouhard/expandable-card-container/)

### Styling
The following custom properties and mixins are available for styling:

| Custom property | Description | Default |
| ----------------|-------------|---------- |
| `--card-width` | Width of the card when retracted | `300px` |
| `--card-height` | Height of the card when retracted | `200px` |
| `--card-font-size` | Font size of the card | `3em` |
| `--card-color` | Card global color | `#000` |
| `--card-button-background-color` | paper-button background color | `#fff` |
| `--card-background-color` | Background color of the card | `#fff` |
| `--card-header-background-color` | Background color for the header when the card is expanded | `#607D8B` |
| `--card-header-color` | Header color | `#fff` |
