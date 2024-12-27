# Custom YouTube Theme for Firefox

This works by overwriting YouTube's CSS using Firefox's `userContent.css` file.

## Previews

Tokyo Night
![Tokyo Night](./previews/tokyonight-preview.webp)

Catppuccin
![Catppuccin](./previews/catppuccin-preview.webp)

## Installation

### Enable User Stylesheets

1. Open Firefox.
2. Type `about:config` into the address bar and press Enter.
3. Click **Accept the Risk and Continue** if prompted.
4. In the search bar, type `toolkit.legacyUserProfileCustomizations.stylesheets`.
5. Set the preference to `true` by double-clicking it.

### Open Profile Directory

1. Type `about:support` into the address bar and press Enter.
2. In the **Application Basics** section, locate **Profile Directory**.
3. Click the **Open Directory** button next to **Profile Directory**.

### Add the Custom CSS Files

1. In your profile directory, create the `chrome` directory if it doesn't exist.
2. Place the following into the `chrome` directory:

* `userContent.css`
* `youtube.css`
* `themes`

### Change the Theme

1. Open `youtube.css` in a text editor.
2. At the top, you'll see this import: `@import url(./themes/tokyonight-night.css);`
3. Edit the import URL to your desired theme.
4. For example: `@import url(./themes/catppuccin-mocha.css);`

### That's it

Close and reopen Firefox for the changes to take effect.
