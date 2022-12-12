```diff
Sidebar Logo - Subpack
```
![MasterHead](https://media.discordapp.net/attachments/1050591171921072130/1051979700660076655/banner.png?width=1011&height=569)
--- ---
```diff
Sidebar Logo a addon that adds a logo or image to the top of
your sidebar. Changing the position of the 'title' and 'actionbar'
while displaying a logo on top for branding.
```

### Change Sidebar Logo
#1 Open ^com.mojang^ folder, in %Appdata%.
#2 Open ^resource_packs^ folder
#3 Open ^sidebar logo^ Folder
#4 Open ^textures/ui/sidebar^ Folder
#5 In the ^sidebar^ testures folder there is a sample ^logo.png^ 
#6 Copy and Paste your [ Logo/Image ] into the ^sidebar^ textures folder
#7 Delete the sample Image and remane your [ Logo/Image ] to ^logo.png^

### [ sidebar supports 75x75 images/logoes ]
```diff
This can be chnages in file pathing com.mojang/resource_packs/sidebar logo/subpacks/{actionbar}or{title}/ui/hud_screen.json/"sidebar:display_logo":
```
```json
{
// Code located in the packs hud_screen.json file.
"sidebar:display_logo": {
    "type": "image",
    "texture": "textures/ui/sidebar/logo",
    "anchor_from": "right_middle",
    "anchor_to": "right_middle",

    // Below is the image/logos main size you can change. 
    "size": [75, 75],

    "offset": [-9, -15],
    "layer": 50
},
```
--- ---
### Display Title
`/title @a title test!`
`/titleraw @a title {"rawtext":[{"text":"test"}]}`

### Display Actionbar
`/title @a actionbar test!`
`/titleraw @a actionbar {"rawtext":[{"text":"test"}]}`

+ Type these commands in chat and create your own personal sidebar!
For more commands or to display scores on your sidebar look below.

### Display Score 
`/titleraw @a title {"rawtext":[{"text":"Balance: "},{"score":{"name":"*","objective":"money"}}]}`

### Display Player 
`/titleraw @a title {"rawtext":[{"selector":"@s"},{"text":" §aIs Broke!"}]}`

### Display Seprate Lines
`/titleraw @a title {"rawtext":[{"text":"Line 1"},{"text":"\nLine 2"}]}`

**NOTE** 

```diff 
- This pack should not be replicated in any way. DONT sell this pack in any way. This debug ui addon can be added to your own pack. Make sure to add credit in the files or in your world! -
```
Replace UUIDs in the packs ^manifest.json^ UUID Generator Link - https://www.uuidgenerator.net/
