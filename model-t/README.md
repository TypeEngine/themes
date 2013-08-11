## SASS Compilation
SASS files are included in this theme in case you'd like to use CSS pre-processing. In your compiler (we use Codekit), set the style.scss file to compile to /featured-article/assets/css/style.css, then set all other SCSS files to not compile directly. The style.css file is the only one delivered to the template.

## Targeting the Largest Viewport
Our CSS assumes that we are targeting the largest viewport, the iPad in landscape orientation. Use media queries to target smaller viewports. Model T has a file specifically for handheld portrait overrides (in this case viewports 479px and narrower – effectively the iPhone and iPod Touch).

This seems counterintuitive with the rise of Mobile First design. However one key thing to remember is that Newsstand issues are download as a single file, so once the device is rendering your files, there is no concern about unused assets being loaded remotely – the assets are already on the device.

## Footnotes
To use footnotes in an article using this theme, the following markup is needed in your article:

```html
<a href="#1" id="footnote1" class="footnote">1</a>
```

Then the corresponding footnote content:

```html
<p>
	<a href="#footnote1" id="1" class="footnote">1</a>
	This is the content of the footnote.
</p>
```

## Author Images
Author images are set to display at a maximum of 200px wide in Model T. This means that author images should be uploaded at 400px wide to ensure sharp rendering on retina screens. Images wider than 400px are unnecessary and will only slow your issue's download speed.

## Variables
Use the variables.scss file to dramatically change the typography, overall margins, and color scheme without affecting the guts of the theme's CSS.

