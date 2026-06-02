<h1 align="center" style="color:#8c1eff">Danwave <br/><br/>


  <img src="https://img.shields.io/visual-studio-marketplace/i/TheCodemonkey.synthwave-x-fluoromachine-epic-animations?color=%23740c5f&logo=visualstudio&logoColor=%23740c5f&style=flat-square"/>
  <img src="https://img.shields.io/visual-studio-marketplace/d/TheCodemonkey.synthwave-x-fluoromachine-epic-animations?color=%23740c5f&logo=visualstudio&logoColor=%23740c5f&style=flat-square"/>
    <img src="https://img.shields.io/visual-studio-marketplace/last-updated/TheCodemonkey.synthwave-x-fluoromachine-epic-animations?color=%23740c5f&logo=visualstudio&logoColor=%23740c5f&style=flat-square"/>
</h1> 

<p align="center"><strong>Danwave brings bold neon-inspired animations into VS Code.</strong></p>



<br/><br/>

*Danwave is a continuation of <a href="https://github.com/webrender/synthwave-x-fluoromachine">synthwave-x-fluoromachine</a>, itself inspired by @robbowen's [Synthwave '84 theme](https://marketplace.visualstudio.com/items?itemName=RobbOwen.synthwave-vscode) and @fullerenedream's [Fluoromachine](https://colorsublime.github.io/themes/FluoroMachine/) for VS Code.*

<br/>

<p align="center">
  <img src="https://user-images.githubusercontent.com/1646017/136690694-79e9973b-6d55-40cb-b8d1-4820d2a4ee35.gif" /><br/>
  <i style="font-size: .8em">legendary TRON underground</i>
</p>
<br/><br/>
<p align="center">
  <img src="https://user-images.githubusercontent.com/1646017/136690891-7bcca587-9489-4a40-ba78-e3b851624dd8.gif" /><br/>
  <i  style="font-size: .8em">epic neon glowing tooltips and folding effects</i>
</p>

<br/>

## Installation 

1. Install this theme  
2. Install [Custom CSS and JS Loader](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css)  
3. Link the CSS file from this extension in your .vscode/settings.json: 

```
On Mac it might look something like the snippet below:

{
  "vscode_custom_css.imports": [
    "file:///Users/{your username}/.vscode/extensions/danie.danwave-theme-0.0.1/danwave.css",
    "file:///Users/{your username}/.vscode/extensions/danie.danwave-theme-0.0.1/danwave-transitions.css"
    ]
}

Windows might resemble:

{
  "vscode_custom_css.imports": [
    "file:///C:/Users/{your username}/.vscode/extensions/danie.danwave-theme-0.0.1/danwave.css",
    "file:///C:/Users/{your username}/.vscode/extensions/danie.danwave-theme-0.0.1/danwave-transitions.css"
    ]
}
```

4. `danwave-transitions.css` is optional and adds the animated effects layer.
5. From the command panel, select `Reload Custom CSS and JS`. You'll need to run this command every time vscode updates.


<br/><br/>

## Font
The font being used in the screenshot above is [Operator Mono with Ligatures](https://github.com/kiliman/operator-mono-lig).


<br/><br/>

## Palette workflow
Shared colors now live in `theme-palette.mjs`.

Run `npm run build` after changing the palette. That script:

1. creates `src/danwave.source.css`, `src/danwave-transitions.source.css`, and `src/danwave.source.json` the first time it runs
2. generates `palette.css` with CSS custom properties
3. rebuilds `danwave.css`, `danwave-transitions.css`, and `themes/danwave.json`

This is necessary because the CSS files can use variables directly, but the VS Code theme JSON cannot. The JSON still has to be generated as plain color values.


<br/><br/>

## Contibution
All contributions are welcome, including issues, new docs as well as updates and tweaks, blog posts, workshops, and more.



<br/><br/>

## Contact
Write me on <a href="https://twitter.com/chillya">twitter</a>.


<br/><br/>

## License
i ❤️ MIT
