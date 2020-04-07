# Firefox-Mod

### About:config

|                  Key                   | Value |
| :------------------------------------: | :---: |
| browser.bookmarks.openInTabClosesMenu  | false |
| browser.tabs.loadBookmarksInBackground | true  |
| browser.bookmarks.showMobileBookmarks  | false |
|      browser.tabs.drawInTitlebar       | true  |
|           gfx.webrender.all            | true  |

### Configuración para Firefox 75

-   Open FF Profile Directory (Help > Troubleshooting > Open Dir)
-   Create a dir called `chrome` and put these files in it.
-   `sideberyDynHover` is to be used with the Sidebery extension.

## Dont forget to enable 'toolkit.legacyUserProfileCustomizations.stylesheets' in about:config for your custom themes to work.

### `searchBar.css`

**New search bar with some changes and fixes. Use the new 75.0 version file.**

![alt text](https://i.redd.it/wpubm02rzfr41.png)

Tested on:

```html
Manjaro Linux / Firefox 75.0b10 / Default Dark Theme
```

![alt text](https://i.imgur.com/Hi1ocvT.png)

You can find more in 'userChrome.css'

```css
/* Comment this to show min/max/close buttons. I use OS style firefox plugin. */
#TabsToolbar > .titlebar-buttonbox-container {
	visibility: collapse !important;
}
```

```css
/* Width of the tabs. Change it to 100% to get full 
width style tabs. But it looks funny, make search 
bar transparent so it looks better with full width */
.tabbrowser-tab[fadein]:not([pinned]) {
	max-width: 135px !important;
}
```

![alt text](https://i.imgur.com/8IUIq2g.png)

Blur style search and bookmarks bar. Used the search method found here

Need about:config 'layout.css.backdrop-filter.enabled' = true
and it could require the 'gfx.webrender.enabled' to true. But if it works with the 'backdrop-filter' leave this one.

```
https://www.reddit.com/r/FirefoxCSS/comments/ddi4dc/testing_the_backdropfilter_in_the_url_dropdown/
```

![alt text](https://i.imgur.com/bU7ahnk.png)

![alt text](https://i.imgur.com/OasXFqd.png)

I use Flexible space for spacing https://imgur.com/a/Gd82v0H

Linux (blur works too after enabling both options mentioned above).

![alt text](https://i.imgur.com/0pxPFnW.png)
