# XORG "cards" data repo

This is a simple stash for our "cards" records that the renderer at https://mborn.eu/xorg/ uses as its database.

### To edit
To edit, add or expand new or existing "cards," simply open the [cards](https://github.com/XORGanon/cards/edit/main/cards) file for editing, do what you desire, and commit your changes when you're done. While doing so, please mind these few but vital _syntax conventions_ to make sure the renderer keeps working:

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

#### Note
Syntax conventions will be updated as the renderer develops, but I'll take care of upgrading them along with the description above.


