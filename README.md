# Mi configuración de Firefox | Manjaro KDE - Firefox 80.0b6 - Default Dark Theme

### About:config

|                  Key                   | Value |
| :------------------------------------: | :---: |
| browser.bookmarks.openInTabClosesMenu  | false |
| browser.tabs.loadBookmarksInBackground | true  |
| browser.bookmarks.showMobileBookmarks  | false |
|      browser.tabs.drawInTitlebar       | true  |
|           gfx.webrender.all            | true  |
| toolkit.legacyUserProfileCustomizations.stylesheets| true|

### CSS Hacks para cambiar la interfaz de Firefox [Source](https://github.com/MrOtherGuy/firefox-csshacks)

-   Ir a about:profiles
-   Crear un directorio `chrome` y poner los archivos de este repositorio ahí.

```bash
~/.mozilla/firefox/dev-edition-default/chrome
❯ ls
image/  searchBar.css  userChrome.css  userContent.css
```

-   `sideberyDynHover` se usa con la extensión [Sidebery](https://addons.mozilla.org/en-US/firefox/addon/sidebery/).

## :warning: No olvides habilitar 'toolkit.legacyUserProfileCustomizations.stylesheets' en about:config para que tus estilos funcionen.

### `searchBar.css`

**New search bar with some changes and fixes. Use the new 75.0 version file.**

![alt text](https://i.redd.it/wpubm02rzfr41.png)


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
