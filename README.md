# MMM-News-json
A module for MagicMirror<sup>2</sup> that displays news, events or any kind of
information as long as it has a title, an image and a text given in json format.

It is derived from DailyXKCD. Thanks for that!

## Dependencies
  * A [MagicMirror<sup>2</sup>](https://github.com/MichMich/MagicMirror) installation

## Installation
  1. Clone this repo into your `modules` directory.
  2. Create an entry in your `config.js` file to tell this module where to display on screen.
  
 **Example:**
```
 {
    module: 'MMM-News-json',
	position: 'bottom_right',
	config: {
		showTitle: true,
		showImage: true,
		showAltText: true
	}
 },
```

## Config
| **Option** | **Description** |
| --- | --- |
| `updateInterval` | Set to desired update interval (in ms), default is `3600000` (10 hours). |
| `showTitle` | Set to `true` to display the title of the comic. |
| `titleFont` | Set a custom font format, default is `large light bright`. To set the size use one of `xsmall small medium large xlarge`, for boldness one of `thin light regular bold`, and to adjust brightness one of `dimmed normal bright`. |
| `showAltText` | Set to `true` to show the alt text (tooltip on the original comic). |
| `altTextFont` | See `titleFont`, except for this is the formatting of the alt text. |
| `showImage` | Set to `true`, if you want to see the image. |
| `limitComicHeight` | Set to limit the height of the comic (in px), default is `450`. The comic will scroll downwards every few seconds, if it is heigher. |
| `scrollInterval` | How often to scroll long comics (in ms), default is `8000` (every 8 seconds). |
| `scrollRatio` | Set how much of the visible height is being scrolled every time. The value should be between `0.0` and `1.0`, default is `0.8` so it scrolls down by 80%. |
