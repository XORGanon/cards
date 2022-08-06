# XORG "cards" data repository

This is a simple stash for our "cards" that is used as a database by the renderer located at https://mborn.eu/xorg/

### To edit
To edit, add or expand new or existing "cards," open the [cards](https://github.com/XORGanon/cards/edit/main/cards) file for editing, do what you desire, and commit your changes when you're done. While doing so, please mind these few but vital _syntax conventions_ to keep the renderer working:

* Prefix the title with `#` + `space`
* Prefix property entries with `+` + `space`
* Divide property names and values with `space` + `:` + `space`
* Keep one empty line between each "card" and the next

#### Like so
    # Schismogenesis
    + Description : The way in which neighboring entities individuate in a highlighting of their differences.
    + Suite : Belonging
    
    # Semioverse miner
    + Lore : Some metaverse miners call their collectively constructed underworld "The megadungeon": a branching [...]
            
    # Et cetera ...

<p style="padding: 1em; background-color: blue; color: white;"><b>Note:</b> The syntax conventions will be updated as the renderer develops, but I will take care of keeping things integral.</p>


