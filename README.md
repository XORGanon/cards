# XORG "cards" repo
This is a simple stash for our "cards" records that the renderer at https://mborn.eu/xorg/ draws on as its database.

### Editing and syntax conventions
To edit, add or expand new or existing "cards," simply [open the cards file for editing](https://github.com/XORGanon/cards/edit/main/cards), do what you desire, and commit your changes when you're done. While doing so, please mind these few but vital _syntax conventions_ to make sure the renderer keeps working. These will be updated as the renderer develops, but I'll take care of upgrading them along the way.

* Prefix the title property with `#` + `space`
* Prefix other property entries with `*` + `space`
* Divide property names and values with `space` + `:` + `space`
* Just for human readability, keep an empty line between each "card" and the next

### Currently implemented properties
The rendered currently processes the following properties. Since their names are also triggers for their styling, print them exactly like this when you use them. Properties with names other than these will be rendered as plain text without specific styling. Naturally, we can at all times add, remove, rename or otherwise mess with these. 
```
# Title
* Type
* Description
* Lore
* Suite
* Image
* Notes
* WIP
```
### Line breaks
To add line breaks in a property text, e.g. to make a list in a description, type a vertical bar `|` where you want the new line to begin.

### Images
To add images, do three things:

* On your computer still, rename the image file you want to connect to a card. (You cannot rename files once they're uploaded.)
* Upload the image to the [img](https://github.com/XORGanon/cards/tree/main/img) folder by simply dragging it onto there and then committing this change.
* Add an image property line to the card that looks like this: `* Image : imagename.jpg`

### Notes, work in progress
To add a note to a "card" which should show up in the render, use the `* Notes` property. To have a place for storing thoughts etc. that should not be rendered, you can store them in `* WIP` a property.

### Cutoff
To bench some "cards" (i.e. remove them from the deck without having to delete them), you can place them beneath the cutoff mark `-----` (five hyphens), all content following which will be dropped before processing. Bonus: This also means that below the cutoff mark, you can work freely without adhering to the syntax conventions.

### All in all, like so:
```html
# Title : Expansive Foaming
* Description : Fill out a void you find in any space (material, conceptual, ...
* Image : level.png

# Title : Sample card
* Description : To play this card: |1. Do step one |2. Do step two |3. Do step three
* Notes : [Notes to be displayed]
* WIP : thought fragments here

# Title : Semioverse miner
* Lore : Some metaverse miners call their collectively constructed ...

-----

<!-- From here on, nothing will be processed because it's beneath the cutoff mark -->
```

