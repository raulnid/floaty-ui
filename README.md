# Floaty UI

Compact Mode, but it floats. Supports Zen Color Picker and background blur.

## Preview

![Floaty UI demo](./media/demo.avif)

## Settings

![Floaty UI settings](./media/settings.png)

## Install

### Sine

1. Install [Sine](https://github.com/CosmoCreeper/Sine)
2. Go to `Settings > Sine Mods` search for `floaty ui` and click install

### Zen Mods

Waiting for https://github.com/zen-browser/theme-store/pull/1585

### Manual

1. Export your mod list from `Settings > Zen Mods > Export Mods`
2. Edit the exported JSON and add

    ```json
    "mod-floaty-ui": {
      "id": "mod-floaty-ui",
      "name": "Floaty UI",
      "description": "Compact Mode, but it floats. Supports Zen Color Picker and background blur.",
      "homepage": "https://github.com/moktavizen/floaty-ui",
      "style": "https://raw.githubusercontent.com/moktavizen/floaty-ui/refs/heads/main/chrome.css",
      "preferences": "https://raw.githubusercontent.com/moktavizen/floaty-ui/refs/heads/main/preferences.json",
      "readme": "https://raw.githubusercontent.com/moktavizen/floaty-ui/refs/heads/main/README.md",
      "image": "https://raw.githubusercontent.com/moktavizen/floaty-ui/refs/heads/main/media/preview-store.png",
      "author": "moktavizen",
      "version": "1.0.0",
      "tags": [],
      "createdAt": "2025-06-29",
      "updatedAt": "2025-06-29",
      "enabled": false
    }
    ```

    The structure should look like this

    ```json
    {
      "other-mods": {
        // other mods info
      }, // don't forget the comma before
      "mod-floaty-ui": {
        // floaty-ui info
      }
    }
    ```

3. Go to <code>[profile folder](https://docs.zen-browser.app/guides/live-editing#step-1-access-the-profile-folder)</code> and replace the content of `zen-theme.json` with the edited JSON
4. Go to <code>[chrome folder](https://docs.zen-browser.app/guides/live-editing#step-2-create-the-chrome-folder) > zen-themes</code> and create a folder called `mod-floaty-ui`, and place `chrome.css` and `preferences.json` inside of it
5. Restart Zen Browser and enable it from `Settings > Zen Mods`

## Uninstall

1. Go to `Settings > Zen/Sine Mods > Remove`
