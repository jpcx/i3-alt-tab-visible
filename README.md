# i3-cycle-focus

[![NPM](https://nodei.co/npm/i3-cycle-focus.png)](https://nodei.co/npm/i3-cycle-focus/)

Simulates an alt-tab operation for the i3 window manager. Shifts the mouse cursor position to the center of focus. Cycles visible windows only.

## Getting Started

### Prerequisites

+ Node.JS version 8.3.0 or above.
+ i3wm
+ i3-nagbar
+ xdotool

### Installing

```console
npm i -g i3-cycle-focus
```

### Deployment

The command should be bound within the i3 config. This is usually `~/.config/i3/config`. The following lines will bind the script to alt+tab for forward cycling and alt+shift+tab for reverse cycling.

```ini
bindsym Mod1+Tab       exec --no-startup-id i3-cycle-focus
bindsym Mod1+Shift+Tab exec --no-startup-id i3-cycle-focus --reverse
```

## Documentation

Internal documentation [here](https://github.com/jpcx/i3-cycle-focus/blob/0.1.0/docs/global.md).

## Testing

Testing provided by jest:

```console
npm i -d --prefix=$(npm root -g)/i3-cycle-focus
npm test --prefix=$(npm root -g)/i3-cycle-focus
```

_Note: if testing, have at least two windows visible and don't move the mouse._

## Versioning

Versioned using [SemVer](http://semver.org/). For available versions, see the [Changelog](https://github.com/jpcx/i3-cycle-focus/blob/0.1.0/CHANGELOG.md).

## Contribution

Please raise an issue if you find any. Pull requests are welcome!

## Author

**Justin Collier** - [jpcx](https://github.com/jpcx)

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/jpcx/i3-cycle-focus/blob/0.1.0/LICENSE) file for details