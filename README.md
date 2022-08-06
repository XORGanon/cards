# XORG "cards" repo

This is a simple stash for our "cards" records that the renderer at https://mborn.eu/xorg/ draws on as its database.

### Editing
To edit, add or expand new or existing "cards," simply open the [cards](https://github.com/XORGanon/cards/edit/main/cards) file for editing, do what you desire, and commit your changes when you're done. While doing so, please mind these few but vital _syntax conventions_ to make sure the renderer keeps working:

* Prefix the title property with `#` + `space`
* Prefix other property entries with `*` + `space`
* Divide property names and values with `space` + `:` + `space`
* Keep an empty line between each "card" and the next

### Adding images
To add images, do two things:

* Upload the image you want to connect to a card into the [img](https://github.com/XORGanon/cards/tree/main/img) folder, by simply dragging it onto there and then committing this change.
* Add a property line to the card: `* Image : imagename.jpg`

### All in all, like so:
	# Title : Expansive Foaming
	* Description : Fill out a void you find in any space (material, conceptual, ...
	* Image : level.png

	# Title : Semioverse miner
	* Lore : Some metaverse miners call their collectively constructed ...

	# Title : Life-cycle

#### Note
Syntax conventions will be updated as the renderer develops, but I'll take care of upgrading them along with the description above.


