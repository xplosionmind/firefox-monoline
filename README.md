# Firefox Monoline

Place everything of your Firefox toolbar in one single line, similar to modern Safari.

<br>
<br>

## Features

- Remove clutter and make Firefox toolbar as compact as possible
- preserve icons and functionalities for which no keyboard shortcut exists
- non-breaking implementation

![Screenshot light theme](https://user-images.githubusercontent.com/42862428/171851199-7206bfd1-7fab-49b9-9498-58db8ccd3482.jpg)
![Screenshot dark theme](https://user-images.githubusercontent.com/42862428/171851212-4634325b-fc4d-475c-ba03-5b63df011a20.jpg)

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

## Related projects

- Inspired from [one-line-firefox](https://github.com/khuedoan/one-line-firefox 'one-line-firefox GitHub repository')
