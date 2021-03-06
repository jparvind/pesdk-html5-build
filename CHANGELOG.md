# 4.2.3

Fixed
-----------

*   \[[PESDK-1927](https://imglysdk.atlassian.net/browse/PESDK-1927)\] \- Fixed issues that were introduced by changing to the correct `.min.js` fileextension. Non-minified extension is now reintroduced to provide backwards compatiblity for now.

# 4.2.2

Fixed
-----------

*   \[[PESDK-1899](https://imglysdk.atlassian.net/browse/PESDK-1899)\] \- Refactored examples and sized them down
*   \[[PESDK-1924](https://imglysdk.atlassian.net/browse/PESDK-1924)\] \- Added prop-types to static build and not as dependency anymore
*   \[[PESDK-1925](https://imglysdk.atlassian.net/browse/PESDK-1925)\] \- Changed the naming of the JS files in the production build to reflect their status minified status to `*.min.js`

# 4.2.1

Added
-----

*   \[[PESDK-1859](https://imglysdk.atlassian.net/browse/PESDK-1859)\] \- Added better error when license is not a string
*   \[[PESDK-1872](https://imglysdk.atlassian.net/browse/PESDK-1872)\] \- Added examples for ServerUI/NodeUI
*   \[[PESDK-1893](https://imglysdk.atlassian.net/browse/PESDK-1893)\] \- Added npm compatibility when sdk is installed via npm
*   \[[PESDK-1900](https://imglysdk.atlassian.net/browse/PESDK-1900)\] \- Added 'image.uri' field to serialization and deserializer can use it to fetch remote images

# 4.2.0

Fixed
---

*   \[[PESDK-1030](https://imglysdk.atlassian.net/browse/PESDK-1030)\] \- Fixed an issue when editing stickers on iOS Safari in ReactUi
*   \[[PESDK-1186](https://imglysdk.atlassian.net/browse/PESDK-1186)\] \- Fixed an issue where webcam access was broken on Edge
*   \[[PESDK-1193](https://imglysdk.atlassian.net/browse/PESDK-1193)\] \- Fixed an issue when adding a sticker blocked the menu on IE11 in DesktopUi
*   \[[PESDK-1251](https://imglysdk.atlassian.net/browse/PESDK-1251)\] \- Fixed an issue where text was scaled wrong after transform
*   \[[PESDK-1252](https://imglysdk.atlassian.net/browse/PESDK-1252)\] \- Fixed issue where square aspect ratio lead to non identical image width and height in ReactUi
*   \[[PESDK-1438](https://imglysdk.atlassian.net/browse/PESDK-1438)\] \- Fixed an issue where parts of text where missing under certain circumstances in DesktopUi
*   \[[PESDK-1482](https://imglysdk.atlassian.net/browse/PESDK-1482)\] \- Fixed an issue where image output was blank after adding sticker and cropping
*   \[[PESDK-1523](https://imglysdk.atlassian.net/browse/PESDK-1523)\] \- Fixed IndexSizeError when going out of bounds in the canvas sticker toolbar on IE11 in ReactUi
*   \[[PESDK-1535](https://imglysdk.atlassian.net/browse/PESDK-1535)\] \- Fixed an issue where screen was frozen after image export in DesktopUi
*   \[[PESDK-1551](https://imglysdk.atlassian.net/browse/PESDK-1551)\] \- Fixed issue when trying to upload unsupported files in the photoroll in the ReactUi
*   \[[PESDK-1641](https://imglysdk.atlassian.net/browse/PESDK-1641)\] \- Fixed an issue where text controls were cropped at the image boundaries in ReactUi
*   \[[PESDK-1654](https://imglysdk.atlassian.net/browse/PESDK-1654)\] \- Fixed jumping text when going into or leaving text edit mode
*   \[[PESDK-1657](https://imglysdk.atlassian.net/browse/PESDK-1657)\] \- Fixed an issue where text or sticker vanished after changing to brush
*   \[[PESDK-1658](https://imglysdk.atlassian.net/browse/PESDK-1658)\] \- Fixed sprite ordering issue when brush was behind text
*   \[[PESDK-1662](https://imglysdk.atlassian.net/browse/PESDK-1662)\] \- Fixed issue when dragging textfield didn't stop
*   \[[PESDK-1670](https://imglysdk.atlassian.net/browse/PESDK-1670)\] \- Fixed error case when dragging and dropping images from another browser window into library in DesktopUi
*   \[[PESDK-1681](https://imglysdk.atlassian.net/browse/PESDK-1681)\] \- Fixed an issue with duplicate text while color was changed
*   \[[PESDK-1682](https://imglysdk.atlassian.net/browse/PESDK-1682)\] \- Fixed a bug where text appeared twice
*   \[[PESDK-1683](https://imglysdk.atlassian.net/browse/PESDK-1683)\] \- Fixed issue when Text and Sticker disappeared when switching to brush
*   \[[PESDK-1684](https://imglysdk.atlassian.net/browse/PESDK-1684)\] \- Fixed issue when Text is not centered
*   \[[PESDK-1685](https://imglysdk.atlassian.net/browse/PESDK-1685)\] \- Fixed an issue where Brushes were duplicated when Zooming in ReactUi
*   \[[PESDK-1703](https://imglysdk.atlassian.net/browse/PESDK-1703)\] \- Fixed issue where brush moved into in foreground by clicking on text
*   \[[PESDK-1766](https://imglysdk.atlassian.net/browse/PESDK-1766)\] \- Fixed a bug where menu overlay background was not showing on IE in the DesktopUi
*   \[[PESDK-1767](https://imglysdk.atlassian.net/browse/PESDK-1767)\] \- Fixed a bug where transform tool was not accessible
*   \[[PESDK-1776](https://imglysdk.atlassian.net/browse/PESDK-1776)\] \- Fixed a bug where text font is initially set to serif because it was not updated after loading
*   \[[PESDK-1788](https://imglysdk.atlassian.net/browse/PESDK-1788)\] \- Fixed bug where requestAnimationFrame was not bound to window when generating stylesheets
*   \[[PESDK-1789](https://imglysdk.atlassian.net/browse/PESDK-1789)\] \- Fixed issue where editor.deserialize(state) did not return Promise as stated in docs
*   \[[PESDK-1802](https://imglysdk.atlassian.net/browse/PESDK-1802)\] \- Fixed bug where requestAnimationFrame was not bound correctly to window


Changed
-----

*   \[[PESDK-1656](https://imglysdk.atlassian.net/browse/PESDK-1656)\] \- Changed behaviour of text-dropdown menu when there is only 1 option
*   \[[PESDK-1860](https://imglysdk.atlassian.net/browse/PESDK-1860)\] \- Refactored SDK into packages/modules, such that every tool can be loaded as needed (see docs)


Added
-----

*   \[[PESDK-1192](https://imglysdk.atlassian.net/browse/PESDK-1192)\] \- Added PNG Fallback for SVG sticker to account for IE11 issues
*   \[[PESDK-1203](https://imglysdk.atlassian.net/browse/PESDK-1203)\] \- Added reset button to adjustment tool in DesktopUi
*   \[[PESDK-1579](https://imglysdk.atlassian.net/browse/PESDK-1579)\] \- Added api documentation for all emumerations
*   \[[PESDK-1749](https://imglysdk.atlassian.net/browse/PESDK-1749)\] \- Added support for React 16.02 and shipping it as default version
*   \[[PESDK-1752](https://imglysdk.atlassian.net/browse/PESDK-1752)\] \- Added Text Background Color Option to DesktopUI
*   \[[PESDK-1765](https://imglysdk.atlassian.net/browse/PESDK-1765)\] \- Added possible to check for changed in the OperationStack (see api docs)
*   \[[PESDK-1777](https://imglysdk.atlassian.net/browse/PESDK-1777)\] \- Added TextMetrics to the SDK thus allowing more accurate Text Rendering (see docs)
*   \[[PESDK-1803](https://imglysdk.atlassian.net/browse/PESDK-1803)\] \- Added option to transfer JFIF header / DPI metadata from original to exported image


# 4.1.5

## Fixed

* Fixed bug when deserialisation in DesktopUI did not return a promise

# 4.1.4

## Fixed

* Fixed bug in RequestAnimationFrame polyfill which cause an  `illegal invocation` error

# 4.1.3

## Fixed

* Fixed `selective-blur` feature

# 4.1.2

## Fixed

* Fixed mip-maps not being re-generated when using `smoothDownscaling` and changing input image

# 4.1.1

## Fixed

* DesktopUI: Fixed switch to default control causing an uncaught exception when initial image needs
  to be resized

# 4.1.0

## Fixed

* ReactUI: Fixed default options for force controls feature
* ReactUI / DesktopUI: Fixed some IE9 bugs
* ReactUI / DesktopUI: Fixed text scaling issues in combination with transform tool
* ReactUI: Fixed sticker and text selection
* ReactUI: Fix text edit mode default text
* DesktopUI: Fixed transitions for slow browsers
* DesktopUI: Fixed brush size when zooming

## Changed

* ReactUI / DesktopUI: Pre-rotate text using Canvas2D for more crispy pixels

# 4.0.4

## Fixed

* Fix stickers being drawn over default stickers when loading stickers from external resource
  and setting `replaceCategories` to `true`.

# 4.0.3

## Fixed

* Fixed force controls not working when image is changed
* Fixed text sprite anchor in ReactUI
* Fixed tinted frames not clearing intermediate buffer when using canvas renderer
* Fixed transform controls not working when canceling switching controls
* Fixed sticker categories loaded from external source not taking `replaceCategories` option into
  account
* Fixed default category label for frame categories
* Fixed sticker category label translation
* Fixed stickers not being re-scaled when image with different dimensions is loaded

# 4.0.2

## Fixed

* Fixed deserialization
* Fixed shapes in IE11
* DesktopUI: Invalid HEX color values are handled correctly now

## Changed

* ReactUI: Better initial sticker dimensions
* Changed default names for shape stickers

# 4.0.1

## Fixed

* Transform control works again

# 4.0.0

PhotoEditorSDK for HTML5 v4.0.0 comes with an all-new user interface designed
and optimized for desktop browsers!

This version contains many API changes. Please refer to our documentation for
the new API: Click [here](https://docs.photoeditorsdk.com/guides/html5/v4-ReactUI)
for the ReactUI and [here](https://docs.photoeditorsdk.com/guides/html5/v4-DesktopUI)
for our new DesktopUI.

**Please note:** With version 4.0.0, you will need to pass in your license file
as a string using the `license` option - both to our UIs as well as the SDK
itself (in case you're using the PhotoEditorSDK class manually). You can obtain
your license, please sign in on our [website](https://www.photoeditorsdk.com/login).

## Added

* Our UIs now have the ability to load custom font faces from .woff files
* Added a new `overlay` operation that places an asset onto the image with
  a specific blend mode
* Added two new blur operations: `gaussian` (blurs the whole image) and `linear`
  (linear gradient blur). The previous `linear` blur is now called `mirrored`.
* Added a 3D Lookup Table filter that can apply color filters using a 3D LUT
  image. All our default filters are based on this technology now. This also
  means that you can now use your iOS and Android filters on HTML5 as well.
  Please refer to our [documentation](https://docs.photoeditorsdk.com/guides/html5/v4-DesktopUI/features/filters)
  to learn more about this feature and how to create your own filters.
* Added a new serialization format (3.0.0) which has been designed for cross-
  platform serialization.
* Our new UI adds controls for various new internal features such as sticker
  opacity and sticker tinting.

## Changed

* Replaced our default sticker packs with two new sticker packs: `emoticons`
  and `shapes`
* `linear` focus is now called `mirrored`

## Known bugs

* Serialization definition is not final yet
* SVG Stickers don't work in IE11


# 3.6.17

## Fixed

* Fixed sticker category selection


# 3.6.16

## Fixed

* Fixed mipmap generation when texture dimensions change from POT to non-POT
* Zoom is now reset to previous level when leaving controls
* Added workaround for Safari WebGL bug when using SVG stickers

## Added

* Add translation key for zoom

# 3.6.15

## Fixed

* Fixed stickers not resized correctly when `fixedRatio` is set to `false`

# 3.6.14

## Editor

* Added `snapRotation` and `snapRotationTolerance` to sticker controls. These options allow you
  to specify values for rotation snapping. `snapRotation` defines the rotation interval (in degrees)
  at which the rotation should snap while `snapRotationTolerance` defines the tolerance around the
  `snapRotation` at which it should snap.
* Fixed exposed `ReactComponent`. For an example on how to use it, [click here](https://github.com/imgly/pesdk-react-demo).

# 3.6.13

## Editor

### Bugfixes

* Fix text and sticker items not draggable when brush has been drawn on top of them

# 3.6.12

## Editor

### Bugfixes

* Fix cross origin issue when using frames
* Fix crop rotation when no crop ratio is selected

# 3.6.11

## Editor

### Bugfixes

* Fixed `editor.controlOptions.crop.selectableRatios` option

# 3.6.10

## Editor

### Bugfixes

* Fixed a bug that caused text items to switch text when being taken to front
* Fixed a bug that caused foreground and background color to not get updated when switching between
  text items

# 3.6.9

## Editor

### Bugfixes

* Fixed sticker loading from external JSON
* Sticker category labels are not resolved using the language objects anymore. Instead, it's using
  the `label` property of a category
* Base URL is no longer prepended to absolute asset URLs

# 3.6.8

## Editor

### Bugfixes

* Fix a bug that caused sticker controls to break when switching between stickers
* Fix a bug that caused editor to crash when exiting the crop control after clicking the `original`
  option
* Hide crop straighten control when `original` option is active

# 3.6.7

## Editor

### Bugfixes

* `smoothDownscaling` option now works propertly again for both the editor and stickers

# 3.6.6

## Editor

### Bugfixes

* Fix force crop / force controls

# 3.6.5

## Editor

### Bugfixes

* Fix SVG filters in combination with `<base>` tags

# 3.6.4

## Editor

### Bugfixes

* Fix rotation not being applied when cropping the whole image

# 3.6.2

## Editor

### Bugfixes

* Fix text height calculation in Firefox < 45.0

# 3.6.1

## Editor

### Features

* New frames feature replaces the old border feature
* We got rid of the "apply" button - instead, we introduced "Default" options for all controls
* Only one focus operation is allowed at a time, so we updated the focus controls
* Font list is now scrollable
* Google Fonts are preloaded correctly, making sure the font previews are rendered correctly
* Displaying a warning when font loading fails
* Don't reload fonts every time the text controls are opened

### Bugfixes

* Crop ratios are now grouped correctly
* Fix crop assets preloading
* Fix text height calculation
* Rotating a crop with fixed pixel values does no longer flip the crop

## SDK

### Bugfixes

* Fix crop with pixel values
* Fix export of transparent images, un-premultiply alpha
* Fix gamma rendering in combination with brightness and contrast

# 3.6.0

## Editor

:rotating_light: **Please note:** From this version on, you will need an API key to use PhotoEditorSDK
for HTML5. Please [log in to your account](https://www.photoeditorsdk.com) to obtain an API key and
specify it using the `apiKey` option.

### Features

* Implement licensing check and `apiKey` option

### Bugfixes

* Fix filter history / undo
* Fix text height calculation (now uses DOM element measuring when available)
* Fix crop and rotation compensation for sprites
* Fix very small brushes
* Fix splash screen assets being preloaded incorrectly

## Engine

### Bugfixes

* Fix a bug that caused Quads to be disposed incorrectly

## SDK

### Bugfixes

* Fix selective blur feature in combination with other texture units
* Fix selective blur for canvas

# 3.5.3

* Removed React and ReactDOM dependencies from source code, they now need to be installed manually.

# 3.5.2

## Editor

### Features

* Add an optional `Selective Blur` feature that allows users to blur parts of the image using a
  brush. Can be enabled using `editor: { tools: ['selective-blur'] }`.
* Add an optional `Gamma correction` feature under `Adjustments`. Can be enabled using
  `editor: { tools: ['gamma'] }`.
* Due to changes to our feature set, our serialization schema has been updated to version `1.0.1`.
  The new `schema.json` can be found [here](http://static.photoeditorsdk.com/serialization/schema-1.0.1.json).
* Decrease brush step, making large brushes look smoother
* Add output dimensions to crop control
* Allow `dimensions` option for crop ratios, causing the resulting image to be exactly of the given
  dimensions (Needs to be a `PhotoEditorSDK.Math.Vector2`)
* Add a preloader (can be disabled using the `editor.preloader` option)

### Bugfixes

* Fix crop rotation deserialization issues
* Fix `smoothUpscaling` option for intermittent render textures
* Fix knob dragging of linear focus controls

## SDK

### Features

* Add `dimensions` option (of type `PhotoEditorSDK.Math.Vector2) to `CropOperation`
* Add `gamma` option to `AdjustmentsOperation`

### Bugfixes

* Fix SDK disposal (`PhotoEditorSDK#dispose` now correctly disposes all textures and shaders)

## Engine

### Bugfixes

* Only use `highp` shader precision when it's available


# 3.5.1

This version of PhotoEditorSDK for HTML5 contains a *lot* of memory management improvements, fixing
a lot of exporting issues and slowdowns on slower / older devices.

## Editor

### Features

* Implement Google Fonts support
* Add `editor.smoothUpscaling` option (default: `false`)

### Bugfixes

* Fix brush texture dimensions while drawing
* Fix brush size when entering tool after zooming in
* Fix webcam button on photo roll screen
* Fix text cropping
* Fix crop ratio remember function
* Fix rounding issues causing textures to be re-initialized
* Fix text selection bug when zoom is larger than 100%
* FilterOperation was not removed when Original Filter was selected
* Fix a bug that caused brushes to disappear after clicking the canvas on retina devices
* Fix brush thickness after crop
* Don't show drag cursor on canvas if image is not draggable
* Correctly set texture quality on export

## SDK

### Bugfixes

* Correctly set texture quality on export
* Fix GLSL randomness function on Mobile Safari
* Operation: Fix RenderTexture disposal
* WebGLFilterManager: Fix RenderTexture disposal
* Shader: Correctly dispose vertex and fragment shaders
* LookupTableFilter: Fix texture disposal
* Dispose render textures before exporting
* Fix PrimitivesStack (Filter) disposal
* Disable operation cache during export, free memory after rendering operation
* Fix SpriteOperation leaking textures

### Features

* Add `editor.smoothUpscaling` option (default: `false`)

### Improvements

* Re-use path canvases

## Engine

### Features

* Automatically add float precision to shaders, depending on platform

# 3.5.0

Breaking changes are tagged with :rotating_light:

## Editor

### Features

* Editor now uses smaller textures while editing which has a **huge** impact on performance when
  using larger images
* Add `editor.forceControls` option. See [the documentation](https://www.photoeditorsdk.com/documentation/html5/editor/force-controls)   for more info.
* Add an overlay bar for text elements with delete and edit buttons (Edit button only appears on
  mobile browsers)
* Zoom now has new zoom levels, similar to Photoshop
* Sticker controls: Add `fixedRatio` option (default is `true`)
* :rotating_light: Crop controls: Renamed `additionalRatios` to `ratios`

### Improvements

* Add brush opacity back in, now behaving correctly
* Improve brush performance
* Photo roll now looks better on mobile browsers

### Bugfixes

* Stickers and texts are selected on click, not on mousedown
* Fix touch event handling on Android
* Fix a crop display bug in Internet Explorer
* Crop is now correctly repositioned when flipping the image

## SDK

### Features

* :rotating_light: All operations: All position values are now relative (0...1) instead of pixel
  values. :rotating_light:
* Add `textureQuality` option
* Add `export.fileBasename` option
* Add `export.quality` option (only works with image/jpeg mime type)

### Bugfixes

* PhotoEditorSDK no longer tries to `require('gl')` and `require('canvas')`, fixing usage in
  Meteor environments
* Fix transparent images getting a white background when filters are applied (WebGL only)

---

# 3.4.2-1

## Editor

### Bugfixes

* Fix upload and webcam icons in photo roll
* Fix `undefined` value in photo roll search input

---

# 3.4.2

## Editor

### Features

* New crop UI with smooth rotation
* Implemented serialization and deserialization

### Bugfixes

* Switch to home screen before exporting (this applies text objects that are being edited while
  clicking the export button)
* Fix brushes disappearing when cropping
* Fix unnecessary re-rendering of some components

## SDK

### Bugfixes

* Fix `#setSpriteScale`
* Operations no longer listen for other operations to update (e.g. `SpriteOperation` listening for
  `CropOperation` to change, so that sprite positions can be changed accordingly). Instead, the UI
  calls `crop`, `rotate` and `flip` on operations that need to compensate changes of other
  operations.

---

# 3.4.1

## Editor

### Bugfixes

* PhotoRoll: Fix distribution of photos across columns
* PhotoRoll: Implemented nicer scroll bars
* PhotoRoll: Fix icon dimensions on retina screens
* Fix repositioning of text objects when image is flipped
* Error messages disable the editor while they're open
* Re-added sticker options bar (flipping, take to front, remove)
* Switching back to home screen when text has been removed
* Fix texts not being deleted

---

# 3.4.0

Please note that this release changes the names of quite a few API methods and options. Please
refer to our current documentation in case you experience any issues with this release.

## Editor

### Features

* New Photo Roll feature that lets your users pick from a variety of photos
* Implemented new splash screen
* Added `showHeader` option
* Added `showTopBar` option
* Added thickness presets for brushes
* Implemented `ReactUI#export` to manually trigger export
* Implemented `ReactUI#setImage` to change the image that's currently being edited
* Color pickers close automatically when clicking outside of a picker
* New text elements automatically clear their contents when edited for the first time (removing
  the default placeholder)
* Re-structured options hash
* EXIF orientation is now handled by a separate `ExifOrientationOperation` so that it doesn't
  interfere with the `OrientationOperation`
* Make K1, K2, K6 and KDynamic filters available via the UI again
* Developers are now allowed to override single localization strings
* Refactored all controls, allowing controls to have their own top-bar controls

### Bugfixes

* Fixed a retina issue that caused the editor to export images with extremely large dimensions
* Fixed default font selection for text tool
* Fixed file picker not working when selecting the same file twice
* Fixed editor in IE9
* Add sub header for webcam screen back in

## Backend

### Features

* Added Clarity, Exposure, Shadows and Highlights to adjustments
* Added `LUTFilter` which uses the same filter technology we use in iOS and Android
* Brushes are now part of SpriteOperation, allowing other sprites to be layered on top of brushes
* Brushes can now have a hardness (a value between 0 (blurry) to 1 (hard))
* Reworked brush drawing, allowing to draw brush images other than circles
* Added context creation error reporting
* Added WebGL framebuffer error reporting
* Added a `smoothDownscaling` option that will enable mip-mapping in WebGL and a smooth resizing
  algorithm in Canvas2D
* Implemented `setSpriteScale` which allows the developer to export images at a specific scale.
  The sprite scale is incorporated in export while zoom level is not.
* Many refactorings, e.g. introducing `Constants.OPTION_TYPE`, `Constants.UNIFORM_TYPE` and
  `Constants.RENDERER_TYPE` objects for cleaner code.

### Bugfixes

* Fixed memory leaks in all operations
* Fixed textures of images where `width` and `height` properties have been changed
* Fixed retina performance issues
