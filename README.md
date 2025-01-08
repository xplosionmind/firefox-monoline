# 🦊 Firefox Monoline

Minimize your Firefox toolbar to **one single line**.

## 🛑 No longer maintained 🛑

I am no longer maintaining this repository, for three reasons.

- I am happily using the gorgeous [Firefox GNOME theme](https://github.com/rafaelmardojai/firefox-gnome-theme 'firefox-gnome-theme repository on GitHub, by Rafael Mardojai'), and I am sticking with it, for the moment.
- Unfortunately, as I am not using this theme myself I do not have enough time to properly tinker with this, and I would prefer [to prioritize other projects](https://codeberg.org/tommi?tab=repositories 'My repositories on Codeberg').
- I found [Firefox Onebar](https://git.gay/freeplay/Firefox-Onebar 'Firefox-Onebar repository on git.gay, by freeplay') to be a much more advanced and up-to-date choice, hence I would prefer to adopt and potentially contribute to that project if I ever switched back to single-line Firefox layout.

## Features

- 🧹 Remove clutter and make Firefox toolbar as essential as possible 🚀
- 🚗 Compact mode support
- ⚠️ Preserve icons and functionalities for which no ⌨️ keyboard shortcut exists
- ✅ Non-breaking implementation
- 💡 Do you have a suggestion? Share it [here](https://github.com/xplosionmind/firefox-monoline 'Firefox Monoline issues on GitHub'))!

![firefox-monoline-preview](https://user-images.githubusercontent.com/42862428/172017568-f908f7ae-5a2a-46fe-a43c-3d2ae2edbb79.gif)

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

This repository is [hosted on Codeberg](https://codeberg.org/tommi/firefox-monoline 'Firefox Monoline repository on Codeberg'), and it is mirrored on [GitHub](https://github.com/xplosionmind/firefox-monoline 'Firefox Monline repository on GitHub'), where [issues](https://github.com/xplosionmind/firefox-monoline/issues 'Firefox Monoline issues on GitHub') are tracked.

## 🕷 Bugs

Report bugs [here](https://github.com/xplosionmind/firefox-monoline/issues 'Firefox Monoline issues on GitHub').

## 🧐 Related projects 👀

- Mainly inspired from [one-line-firefox](https://github.com/khuedoan/one-line-firefox 'one-line-firefox GitHub repository')
- [Oneline Proton](https://github.com/newmanls/OnelineProton 'Oneline Proton source code on GitHub')
- [Firefox-Onebar](https://codeberg.org/Freeplay/Firefox-Onebar 'Firefox-Onebar source code on Codeberg')
