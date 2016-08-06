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

Its not really possible to think of all the usecase for this type of component.
Hence, you should really customize it to fit your needs.
Maybe you want another element of your card to be animated instead of the header while expanding,
or maybe you want to pass an image property for your card.
Dont be afraid to tweek this component as you want.

`expandable-card` by itself is not very useful, because you will probably want
to use more than one. To get multiple `expandable-card` that expands to fit a container
see [expandable-card-container](https://customelements.io/willydouhard/expandable-card-container/)

### Styling
The following custom properties and mixins are available for styling:
Custom property | Description | Default |
----------------|-------------|---------- |
`--card-width` | Width of the card when retracted | `300px` |
`--card-height` | Height of the card when retracted | `200px` |
`--card-font-size` | Font size of the card | `3em` |
`--card-color` | Card global color | `#000` |
`--card-button-background-color` | paper-button background color | `#fff` |
`--card-background-color` | Background color of the card | `#fff` |
`--card-header-background-color` | Background color for the header when the card is expanded | `#607D8B` |
`--card-header-color` | Header color | `#fff` |
@demo demo/index.html
