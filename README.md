# Extension audio / soundpack

## Info
Wodking directory for the soundpacks are `public/assets/ui-packs`

# Adding a Soundpack
1. Navigate to the `public/assets` folder and create a directory named `ui-packs` if it doesn't already exist.
2. Extract the contents of a zip file into this `ui-packs` directory, or create a new soundpack folder.
3. Go to SillyTavern and access **Extensions > Dynamic Audio > UI config > select a pack at the top > Save and Apply**.
4. Test by clicking on buttons and moving your mouse over them to experience the added audio effects

# Creating your own Soundpack
1. Begin by creating a new folder within the `public/assets/ui-packs` directory.
2. Inside this folder, create a file named `manifest.json` with the following contents:
```
{
    "name": "Example Pack"
    "description": "Example",
    "icon": "icon.png",
    "author": "Everyone",
    "click_behaviour": "single",
    "hover_behaviour": "single",
    "file_onclick": "click/UI_Click.ogg",
    "files_onclick": [],
    "file_onhover": "click/UI_Hover.ogg",
    "files_onhover": []
}
```

## Behaviours
### `single` / `multiple`
- When set to `single`, only one audio be played

- You can set both `click_behaviour` and `hover_behaviour` to either `single` or `multiple`.<br>
When set to multiple, the `files_onclick` or `files_onhover` will take effect. You can customize paths like `foo/bar.mp3`

> [!WARNING]
> Only browser-supported audio formats like `mp3`, `wav`, `ogg`, and similar are playable.
> 
> When clicking or hovering, the current time on the audio will be set to 0 seconds

### `conditional`
Conditional will come soon



