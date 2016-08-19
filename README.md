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
<expandable-card>
      <!-- Content displayed when retracted -->
    <div id="retracted" class="container">
	    <paper-card heading="Retracted title">
		    <div class="card-content">Retracted content</div>
		    <div class="card-actions">
				    <paper-button class="toggle" noink>Expand</paper-button>
		    </div>
	    </paper-card>
    </div>

    <!-- Content displayed when expanded -->
     <div id="expanded" class="container">
		<div id="expandedHeader" class="container-header">
			<paper-icon-button class="container-header-side toggle" noink icon="arrow-back"></paper-icon-button>
			<div>Expanded title</div>
			<div class="container-header-side"></div>
		</div>
		<div id="expandedContent">Expanded content</div>
     </div>
</expandable-card>
```

Add a toggle class to the elements who are supposed to trigger a toggle.
You can custom the titles and contents as you wish.

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
