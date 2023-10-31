# 🦊 Firefox Monoline

Minimize your Firefox toolbar to **one single line**.

![firefox-monoline-preview](https://user-images.githubusercontent.com/42862428/172017568-f908f7ae-5a2a-46fe-a43c-3d2ae2edbb79.gif)

## Features

- 🧹 Remove clutter and make Firefox toolbar as essential as possible 🚀
- 🚗 Compact mode support
- ⚠️ Preserve icons and functionalities for which no ⌨️ keyboard shortcut exists
- ✅ Non-breaking implementation
- 💡 Do you have a suggestion? Share it [here](https://github.com/xplosionmind/firefox-monoline 'Firefox Monoline issues on GitHub'))!

## 🧑🏻‍💻 Usage

- visit `about:config`
  - set `toolkit.legacyUserProfileCustomizations.stylesheets`: `true`
  - `extensions.pocket.enabled`: `false`
- Go to Menu > More Tools > Customize Toolbar:
  - auto-hide downloads button
  - remove all flexible space
  - remove all icons
- Open `about:support`, copy the path of the Profile Folder
- open the terminal
- run `cd /path/to/profile`
- run `git clone https://codeberg.org/tommi/firefox-monoline.git chrome`

### 🚗 Compact mode

The built-in Firefox “Compact mode” vertically compresses the navigation bar by slightly **reducing its height**. To activate it:

1. visit the `about:config` page;
2. search for `browser.compactmode.show` and change it to `true`;
3. go to Menu > More Tools > Customize Toolbar, set density as “compact”.

In order to use Compact mode with <cite>Firefox Monoline</cite> it is necessary to change some parts of [userChrome.css](./userChrome.css):

- remove [the first 9 lines](https://github.com/xplosionmind/firefox-monoline/blob/main/userChrome.css#L1-L9) (delete `urlbar-container` and `urlbar` styling)
- in [line 34](https://github.com/xplosionmind/firefox-monoline/blob/main/userChrome.css#L34), change the value to `-36px !important`

## 👾 Source code

This repository is [hosted on Codeberg](https://codeberg.org/tommi/firefox-monoline 'Firefox Monoline repository on Codeberg'), and it is mirrored on [GitHub](https://github.com/firefox-monoline 'Firefox Monline repository on GitHub'), where [issues](https://github.com/firefox-monoline/issues 'Firefox Monoline issues on GitHub') are tracked.

## 🕷 Bugs

Report bugs [here](https://github.com/xplosionmind/firefox-monoline/issues 'Firefox Monoline issues on GitHub').

## 🧐 Related projects 👀

- Mainly inspired from [one-line-firefox](https://github.com/khuedoan/one-line-firefox 'one-line-firefox GitHub repository')
- [Oneline Proton](https://github.com/newmanls/OnelineProton 'Oneline Proton source code on GitHub')
- [Firefox-Onebar](https://codeberg.org/Freeplay/Firefox-Onebar 'Firefox-Onebar source code on Codeberg')
