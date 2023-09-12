## Guide Functions 

Each part of your guide is seperated by steps like so

```
step
do something
step
do another thing
```

**Popup textbox**

*Ending text with ##Window Title Text will allow custom titles*
```
Format: **popuptext text##WindowTitle**
Example:
Click Here to see youtube video |popuptext https:\\youtu.be/sdsdsds##Example Video
```

**Adding Labels**

```
label "Name_of_Label"
```

**Adding Tips**

```
|tip this is a awesome tip very important information
```

**Quest Functions**

***talk***

   *tells user to talk to npc the number after ## is the npc id*

```
talk Shadow Priest Sarvis##1569
```

***accept***

```
Format: accept Quest Name##QUESTID 
Example: accept Rude Awakening##363
With Goto cords :accept Rude Awakening##363 |goto 30.84,66.20
```

***turnin***

```
Format: turnin Quest Name##QUESTID 
Example: turnin Rude Awakening##363
With Goto cords :turnin Rude Awakening##363 |goto 30.84,66.20
```
