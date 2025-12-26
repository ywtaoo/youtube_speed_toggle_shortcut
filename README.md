# YouTube Speed Toggle

A simple Tampermonkey userscript that adds a speed toggle button to YouTube player controls, allowing you to switch between **1x** and **2x** playback speed with one click.

![YouTube Speed Toggle Demo](https://img.shields.io/badge/YouTube-Speed%20Toggle-red?style=flat-square&logo=youtube)
![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)
![Tampermonkey](https://img.shields.io/badge/Tampermonkey-Ready-green?style=flat-square)

## Features

- **One-Click Toggle** - Switch between 1x and 2x speed instantly
- **Convenient Location** - Button placed in the player control bar, matching native button style
- **Auto Sync** - Automatically syncs with current video speed state
- **SPA Support** - Fully supports YouTube single-page application navigation

## Installation

### Prerequisites

First, install the Tampermonkey browser extension:

- [Chrome / Edge / Brave](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
- [Firefox](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
- [Safari](https://apps.apple.com/app/tampermonkey/id1482490089)

### Install Script

**Option 1: Install from Greasy Fork (Recommended)**

[Click to Install](https://greasyfork.org/en/scripts/560281-youtube-speed-toggle)

**Option 2: Manual Installation**

1. Click the Tampermonkey icon in your browser
2. Select "Create a new script"
3. Delete the default content and paste the contents of [`youtube-speed-toggle.user.js`](youtube-speed-toggle.user.js)
4. Press `Ctrl+S` / `Cmd+S` to save

**Option 3: Install from GitHub Raw**

Click the link below and Tampermonkey will automatically detect and prompt for installation:

[Direct Install](https://github.com/ywtaoo/youtube-speed-toggle/raw/main/youtube-speed-toggle.user.js)

## Usage

1. Open any YouTube video page
2. Find the speed button on the right side of the player control bar (displays "1x" or "2x")
3. Click the button to toggle speed

## Screenshot

The button is located on the right side of the player control bar:

```
[Play/Pause] [Progress Bar] [Volume] [Captions] [Settings] [1x] [Miniplayer] [Theater] [Fullscreen]
                                                            ^^^
                                                        Speed Button
```

## Customization

To modify the available speed options, edit the `SPEEDS` array in the script:

```javascript
const SPEEDS = [1, 2];  // Default: 1x and 2x
const SPEEDS = [1, 1.5, 2];  // Example: Add 1.5x
const SPEEDS = [0.5, 1, 1.5, 2, 2.5];  // Example: More options
```

## Compatibility

- Chrome + Tampermonkey
- Firefox + Tampermonkey
- Edge + Tampermonkey
- Safari + Tampermonkey
- Brave + Tampermonkey

## License

[MIT License](LICENSE)

## Contributing

Issues and Pull Requests are welcome!

## Changelog

### v1.0.0 (2025-12-26)

- Initial release
- Add 1x / 2x speed toggle functionality
- Support YouTube SPA navigation
