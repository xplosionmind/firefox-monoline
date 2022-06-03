# Firefox Monoline

Place everything of your Firefox toolbar in one single line, similar to modern Safari.

<br>
<br>

## Features

- Remove clutter and make Firefox toolbar as compact as possible
- preserve icons and functionalities for which no keyboard shortcut exists
- non-breaking implementation

<br>
<br>

## How to start

- visit `about:config`
  - set `toolkit.legacyUserProfileCustomizations.stylesheets`: `true`
  - `browser.compactmode.show`: `true`
  - `extensions.pocket.enabled`: `false`
- Go to Menu > More Tools > Customize Toolbar:
  - at the bottom, set density as “compact”,
  - auto-hide downloads button
  - remove all flexible space
  - remove all icons
- Open `about:support`, copy the path of the Profile Folder
- open the terminal
- run `cd /path/to/profile`
- run `git clone https://codeberg.org/tommi/firefox-monoline.git chrome`

<br>
<br>

## To do

- [ ] right-align extension icons
	- [ ] create a variable in order to easily change spacing according to how many extensions appear in the toolbar
- [ ] use attributes selectors in order to change spacing according to whether the downloads icon is displayed
- [ ] show some necessary `#titlebar-buttonbox`
- [ ] evaluate behavior with non-compact mode
	- [ ] create a variable to toggle spacing for compact/non-compact mode
- [ ] understand why `#urlbar[breakout][breakout-extend]` `top` and `left` styles do not work.
- [ ] Sass implementation

#### PR

- [ ] Share on awesome repositories
- [ ] Share on design communities

<br>
<br>

## Related projects

- Inspired from [one-line-firefox](https://github.com/khuedoan/one-line-firefox 'one-line-firefox GitHub repository')
