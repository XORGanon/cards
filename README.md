# XORG "cards" data repository

This is a simple dump/stash/data repository for our "cards" that is used as a database by the renderer at https://mborn.eu/xorg/



### To edit
To edit, add, expand, ... new or existing "cards," simply open the [cards](https://github.com/XORGanon/cards/edit/main/cards) file, do what you desire, and commit your changes when you're done.
While doing so, please mind to keep these few but vital **syntax conventions** so that the renderer will keep working:

* Prefix the title with ´´# ´´
* Prefix any property entries with ´´+ ´´
* Divide property names and values with ´´: ´´
* Add one empty line after the entry

##### Like so
    # <TITLE>
    + <PROPERTY>: <PROPERTY_VALUE>
    <BLANK_LINE>

##### Example
    # Schismogenesis
    + Description: The way in which neighboring entities individuate in a highlighting of their differences.
    + Suite: Belonging




