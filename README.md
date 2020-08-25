# Mi configuración de Firefox | Manjaro KDE - Firefox 80.0b6 - Default Dark Theme

### About:config

|                  Key                   | Value |
| :------------------------------------: | :---: |
| browser.bookmarks.openInTabClosesMenu  | false |
| browser.tabs.loadBookmarksInBackground | true  |
| browser.bookmarks.showMobileBookmarks  | false |
|      browser.tabs.drawInTitlebar       | true  |
| toolkit.legacyUserProfileCustomizations.stylesheets| true|

### HW Acceleration on Linux (X11)
|                  Key                   | Value |
| :------------------------------------: | :---: |
|           gfx.webrender.all            | true  |
|       media.ffmpeg.vaapi.enabled       | true  |
|          media.ffvpx.enabled           | false  |

- Exportar la variable `MOZ_X11_EGL=1` (Agregarla al archivo `/etc/environment`)

### [CSS Hacks]((https://github.com/MrOtherGuy/firefox-csshacks)) para cambiar la interfaz de Firefox

![Firefox](https://i.imgur.com/l6TpXkU.png)

-   Ir a about:profiles
-   Crear un directorio `chrome` y poner los archivos de este repositorio ahí.

```bash
~/.mozilla/firefox/dev-edition-default/chrome
❯ ls
image/  searchBar.css  userChrome.css  userContent.css
```

-   `sideberyDynHover` se usa con la extensión [Sidebery](https://addons.mozilla.org/en-US/firefox/addon/sidebery/).

## :warning: No olvides habilitar 'toolkit.legacyUserProfileCustomizations.stylesheets' en about:config para que tus estilos funcionen.
