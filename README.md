Ice Ice OLED
============

Cool-toned, icy colors on a pure black background, optimized for giving you good shivers on an OLED display.

![Ice Ice OLED theme in a dark room](https://github.com/mholt/ice-ice-oled/blob/main/media/photo1.jpg?raw=true)

![Ice Ice OLED theme showing diffs in a dark room](https://github.com/mholt/ice-ice-oled/blob/main/media/photo2.jpg?raw=true)

Theme goals, in order:

- Optimize for OLED
- Legibility (easy to read)
- Immersion (it's easy to get absorbed into the code, to enhance your focus)
- Scanning performance (colors give quick visual cues at a glance, or in your peripheral vision)
- Look cool

I made this theme because I was not completely satisfied with other themes optimized for OLED. My requirements are:

- **Pure black background, for maximum visibility.** In a light room, the extra contrast is essential for legibility. Maxing the brightness and contrast settings on the monitor diminishes OLED longevity, so it's essential that text be legible at lower brightness. I find non-black is wasteful and distracting on OLEDs, and it can increase burn-in risk slightly. Besides, pure black looks _awesome_ in a dark room.
- **Monochromatic&mdash;almost.** Most OLED themes have too many colors; it's noisy, requiring high cognition to scan and interpret mentally, slowing down my productivity. On an OLED, one color does not stand out particularly more than others (except black and white). So monochrome is appealing to me, but other themes take it too far and have only literally a single color.
- **Defined borders.** Lots of themes seem to forget about borders. Makes it hard to drag/resize panes...
- **Accent colors must be pleasant and eye-catching.** Secondary colors, like those used to compare diffs, highlight braces or notes (such as "TODO:" with the help of an extension) should look good in situ, and draw attention&mdash;but not too much.

This theme:

- **Has a pure black background.** Maximum OLED goodness in both light and dark rooms.
- **Uses adjacent colors for syntax.** It's almost monochromatic, but with enough color variety to increase legibility and scanning performance.
- **Has icy, but off-white text.** Pure white on pure black is also too harsh a contrast when used with most text, so it's tempered a bit.
- **Has borders!** Without them being distracting. You will know where to click!
- **Works with some extensions.** It should look nice with GitLens and TODO Highlight.
- **Has a pleasant diff view.** But that's just my opinion.


## Recommended extensions

[GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) makes source control appear directly in your editor, and this theme has color customizations for it.

[TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight) brings attention to certain strings like "TODO:" in your editor. These colors aren't customized by themes, unfortunately, but here's the user settings I use that I think look great with this theme:

![Preview of TODO Highlight colors](https://github.com/mholt/ice-ice-oled/blob/main/media/todo-highlight.png?raw=true)

```json
"todohighlight.keywords": [
	{
		"text": "TODO:",
		"color": "black",
		"backgroundColor": "#eccc3e",
		"overviewRulerColor": "#eccc3e"
	},
	{
		"text": "FIXME:",
		"color": "black",
		"backgroundColor": "#f776a9",
		"overviewRulerColor": "#f776a9"
	},
	{
		"text": "nolint:",
		"color": "#ff80ac",
		"border": "1px solid #ff80ac",
		"backgroundColor": "rgb(0 0 0 / 0)",
		"overviewRulerColor": "#ff80ac"
	},
	{
		"text": "NOTE:",
		"color": "#1bc74c",
		"border": "1px dotted #1bc74c",
		"backgroundColor": "rgb(0 0 0 / 0)",
		"overviewRulerColor": "#1bc74c"
	},
	{
		"text": "BUG:", 
		"color": "#cc0000",
		"border": "1px solid #cc0000",
		"borderRadius": "4px", // NOTE: use borderRadius along with `border` or you will see nothing change
		"backgroundColor": "rgb(0 0 0 / 0)",
		"diagnosticSeverity": "warning", // Set diagnostic severity to `none`, `information`, `warning` or `error`
		"overviewRulerColor": "#cc0000"
	},
	"EXPERIMENTAL:"
]
```