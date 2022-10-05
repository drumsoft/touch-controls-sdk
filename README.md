# touch-controls-sdk

Touch Controls SDK for Scratch 3 - add a "virtual gamepad" / "touch controls" to your project for touch screen (no keyboard) users.

## build

``
npm install
npm run build
``

".sprite3" files is created in sprites directory.

## apply the SDK sprites to your project.

### add sprites

1. Open your project in Scratch ( https://scratch.mit.edu/ ).
1. Point "Choose a Sprite" button and select "Upload Sprite".
1. Select ".sprite3" files in sprites directory (You can select multiple files at once).

### add key events

1. Replace `[when [???] key pressed]` event block with `[when I [receive key-??? pressed]]`. Or make the same code work for both events.

### or add key sensing

1. Replace `<key (???) pressed?>` sensing block with `<([costume #] of (key-???)) = (2)>`. Or concat them in `<<> or <>>` block to work for both input.

`<([costume name] of (key-???)) = (on)>` is also work as key sensing.

## change key designs

1. Edit costumes/scratch-touch-buttons.ai in Illustrator.
1. Export all artboards in SVG format to costumes directory (Illustrator appends /SVG/ in the path).
1. Open svg-test.html to test visibility of SVGs.
1. Build and Install

## manual for scratch users.

Touch Controls SDK for Scratch 3 - add a "virtual gamepad" / "touch controls" to your project for touch screen (no keyboard) users.

Apply Touch Controls SDK to your project.

1. Export the "key-???" sprites you want to use from Touch Controls SDK project.
2. Upload the "key" sprite files to your project.
3. Adjust the layout of the "key" sprites to fit your project.
4. Change the code to respond to the "key" sprites.
  4A. If your code uses [when [???] key pressed] event block, replace it with [when I [receive key-??? pressed]] event block. Or, make the same code work for both events.
  4B. If your code uses <key (???) pressed?> sensing block, replace it with <([costume #] of (key-???)) = (2)> operater block. Or connect these two blocks with an "Or" block so that they both respond.

Since Scratch does not support multiple touches, these "key"s do not support multiple presses. However, by slightly overlapping the 4 arrow "key"s, 8-way control will be possible.

## to upload .sprite3 files on iOS Safari

Since iOS Safari ignores ".sprite3" extension, you cannot upload sprite files in your project.
A bookmarklet that makes sprite files uploadable is available in the link below.

[to upload .sprite3 files on iOS Safari](https://drumsoft.com/sprite3-upload-test.html)
