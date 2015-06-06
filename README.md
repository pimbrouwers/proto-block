## Proto Block: Rapid CSS Prototyping with Blocks

Proto Block is a simple, light-weight (weighing in at ~2kb minified) & extensible foundational css grid. Proto Block does only what it needs to and leave's the rest to you. What makes Proto Block unique is it's usage of relative-sizing for it's grid-base (all values are relative (em, rem, etc.) and based on the 100% 16px base), as well clever usage of font "bumps" to optimize. The intended purpose being the usage of screen real estate & improve UX by increasing legibility across browser-sizes. Proto Block is lovingly crafted and maintained in Toronto, ON.

## What's included

Within the download you'll find the following directories and files, logically grouping common assets and providing both compiled and minified variations. You'll see something like this:

```
proto-block/src/
├── css/
│   ├── reset.css
│   ├── layout.css
│   ├── scaler.css
│   ├── template.css
├── js/
│   └── libs/
│   		└── modernizr-2.5.min.js
└── min/
    ├── proto-block.min.css
    └── js/
        └── libs/
     		└── modernizr-2.5.min.js
```


## How To

Using Proto Block is straight forward. Row's are designated using the "row" class. Row's are comprised of "block" elements (b1, b2, b4, b6, b8, b10, b12). A row's block elements should add up to 12 (ie: b4 - b8 or b6 - b6). By default, row's will expand to fill the entire width of the screen. To prevent full-width layouts simple wrap all rows in a "container" element, which will initalize a "golden" wrap at 960px.

### Full width prototyping (note the usage of ```html<div class="content">..</div>``` for spacing purposes):

```html
<div class="row">
	<div class="block b12">
		<div class="content"></div>
	</div>
</div>
<div class="row">
	<div class="block b6">
		<div class="content"></div>
	</div>
	<div class="block b6">
		<div class="content"></div>
	</div>
</div>
<div class="row">
	<div class="block b4">
		<div class="content"></div>
	</div>
	<div class="block b8">
		<div class="content"></div>
	</div>
</div>
```

###Golden-width prototyping (note the usage of ```html<div class="content">..</div>``` for spacing purposes):

```html
	<div class="container">
		<div class="row">
			<div class="block b12">
				<div class="content"></div>
			</div>
		</div>
		<div class="row">
			<div class="block b6">
				<div class="content"></div>
			</div>
			<div class="block b6">
				<div class="content"></div>
			</div>
		</div>
		<div class="row">
			<div class="block b4">
				<div class="content"></div>
			</div>
			<div class="block b8">
				<div class="content"></div>
			</div>
		</div>
	</div>
```