
:![](https://raw.githubusercontent.com/VictorAlmeidaFonseca/dark-mode/master/assets/dark-icon.png):

# Dark Mode
#### About the dark mode 

Light-on-dark color scheme, also called dark mode, dark theme or night mode, is a color scheme that uses light-colored text, icons, and graphical user interface elements on a dark background and is often discussed in terms of computer user interface design and web design.

 [Wikipedia](https://en.wikipedia.org/wiki/Light-on-dark_color_scheme) - Light-on-dark color scheme

## Guide

![](https://raw.githubusercontent.com/VictorAlmeidaFonseca/dark-mode/master/assets/dark-mode.gif)

First of all, look at **styles.css** file. In this we have the snippet below:

```css
html {
    /* some code  */
    --bg: #fcfcfc;
    --bg-panel: #ebebeb;
    --color-headings: #0077ff;
    --color-text: #333333
}
```
The css variables above store the main page's original color. This variables is necessary for the **main.js** file at repository to manipulate CSS styles via JavaScript on right way. 

Bellow at the **main.js** javascript file we have the object:

```javascript
   const darkMode = {
    bg: "#333333",
    bgPanel: "#434343",
    colorHeadings: "#3664FF",
    colorText: "#B5B5B5"
}
```
This object stores the new colors that will update the css variables handle with global variable, window, representing the window in which the script is running.

As long as you want change the colors, just change the assignments at variables above.
