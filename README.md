# XORG "cards" repo

This is a simple stash for our "cards" records that the renderer at https://mborn.eu/xorg/ draws on as its database.
<br/>
<br/>
<br/>
<br/>

## Editing
### Editing process
To edit, add or expand new or existing "cards," simply [open the cards file for editing](https://github.com/XORGanon/cards/edit/main/cards) and do what you desire. After you're done, commit your changes using the button at the bottom of the page
<br />

### Cutoff
To bench some "cards" without having to delete them, I built in a cutoff mark, all "cards" following which will not be considered by the renderer. The mark is five hyphens: `-----`
<br/>
<br/>
<br/>
<br/>

## "Card" entries
### Syntax conventions
When editing the cards, mind a few but vital _syntax conventions_ to make sure the renderer keeps working:

* Prefix the title property with `#` + `space`
* Prefix other property entries with `*` + `space`
* Divide property names and values with `space` + `:` + `space`
* Keep an empty line between each "card" and the next

(These conventions will be updated as the renderer develops, but I'll take care of upgrading them along with the description above.)
<br/>
<br/>

### Title and properties
The rendered currently knows the following properties. Since their names are triggers for their styling, they should be written as printed here:
* Core properties
  * Title
  * Type
  * Description
  * Lore
  * Suite
  * Image
* Marginal properties
  * Notes
  * WIP
<br/>

### Images
To add images, do three things:

* On your computer still, rename the image file you want to connect to a card. (You cannot rename files once they're uploaded.)
* Upload the image to the [img](https://github.com/XORGanon/cards/tree/main/img) folder by simply dragging it onto there and then committing this change.
* Add an image property line to the card that looks like this: `* Image : imagename.jpg`
<br/>

### Line breaks
To add line breaks, e.g. to make a list in a description, type a vertical bar `|` where you want the new line to begin.
<br/>
<br/>

### Work in progress
To have a place for storing thoughts etc. that won't be rendered out, you can store them in a WIP property: `* WIP : loose thoughts here`
<br/>
<br/>
<br/>
<br/>

## Example
```md
# Title : Expansive Foaming
* Description : Fill out a void you find in any space (material, conceptual, ...
* Image : level.png

# Title : Sample card
* Description : To play this card: |1. Do step one |2. Do step two |3. Do step three

# Title : Semioverse miner
* Lore : Some metaverse miners call their collectively constructed ...

-----

# Title : Life-cycle // This card will not be rendered because it's behind the cutoff mark
```
<br/>
<br/>
<br/>
<br/>




