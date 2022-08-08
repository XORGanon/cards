# XORG "cards" repo

This is a simple stash for our "cards" records that the renderer at https://mborn.eu/xorg/ draws on as its database.
<br/>
<br/>
<br/>
<br/>

## Editing
### Title and properties
To edit, add or expand new or existing "cards," simply [open the cards file for editing](https://github.com/XORGanon/cards/edit/main/cards), do what you desire, and commit your changes when you're done. While doing so, please mind these few but vital _syntax conventions_ to make sure the renderer keeps working:

* Prefix the title property with `#` + `space`
* Prefix other property entries with `*` + `space`
* Divide property names and values with `space` + `:` + `space`
* Keep an empty line between each "card" and the next

So far, the below properties are accounted for in the renderer. They should be written exactly like this, since the property name will be used to attribute styling:
* `# Title : `
* `* Description : `
* `* Lore : `
* `* Suite : `
* `* Notes : `
* `* WIP : `

### Images
To add images, do three things:

* On your computer still, rename the image file you want to connect to a card. (You cannot rename files once they're uploaded.)
* Upload the image to the [img](https://github.com/XORGanon/cards/tree/main/img) folder by simply dragging it onto there and then committing this change.
* Add an image property line to the card that looks like this: `* Image : imagename.jpg`

### Line breaks
To add line breaks, e.g. to make a list in a description, type a vertical bar `|` where you want the new line to begin.

### Work in progress
To have a place for storing thoughts etc. that won't be rendered out, you can store them in a WIP property: `* WIP : loose thoughts here`
<br/>
<br/>
<br/>
<br/>

## File structure

### Cutoff
To bench some "cards" without having to delete them, I built in a cutoff mark, all "cards" following which will not be considered by the renderer. The mark is five hyphens: `-----`
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

---
<br/>
<br/>
<br/>
<br/>

#### Note
Syntax conventions will be updated as the renderer develops, but I'll take care of upgrading them along with the description above.


