# touch-controls-sdk

Touch Controls SDK for Scratch 3 - add a "virtual gamepad" / "touch controls" to your project for no keyboard users.

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
