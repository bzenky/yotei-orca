# Yotei for Orca

A purple-red dawn palette for [Orca](https://www.onorca.dev), with three variants:

| Theme | Base | Appearance |
| --- | --- | --- |
| Yotei | Dark | Original dark palette |
| Yotei Midnight | Dark | Deeper dark palette |
| Yotei Dawn | Light | Soft light palette |

Each theme colors the app, the code editor (syntax colors), and the terminal.

## Install from the plugin directory

Open **Settings → Plugins**, search for **Yotei**, and choose **Install**. Then
open **Settings → Appearance** and pick a variant.

## Install from a local folder

1. Open **Settings → Plugins** and turn on plugins.
2. Choose **Development folders…** and add this folder.
3. Open **Settings → Appearance** and pick **Yotei** or **Yotei Midnight** as the
   dark theme, or **Yotei Dawn** as the light theme. The matching terminal colors
   are offered next to each theme.

You can also load the folder from a terminal:

```sh
orca plugin dev load path/to/this/folder
```

## Build

The files in this folder are generated from the
[VS Code themes](https://github.com/bzenky/yotei/tree/master/visual-studio-code/themes)
in [bzenky/yotei](https://github.com/bzenky/yotei). Don't edit them by hand. After
you change a VS Code theme, rebuild and validate from that repository:

```sh
node tools/build-orca-theme.mjs
orca plugin validate orca
```
