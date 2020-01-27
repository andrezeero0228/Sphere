# LiveG Sphere Browser
Sphere, the web browser designed for the LiveG ecosystem. Bringing you power, speed, functionality and more.

This repository is licensed by the [LiveG Open-Source Licence](https://github.com/LiveG-Development/Sphere/blob/master/LICENCE.md).

Sphere is a web browser which is written in JavaScript using [Adapt UI](https://github.com/LiveG-Development/Adapt-UI) and [Zapr](https://github.com/LiveG-Development/Zapr). The browser is very portable and is supported by a wide range of platforms. Sphere is built on top of [Electron](http://electronjs.org/) so that it is a standalone application which can be packaged into gDesk OS apps, Linux binaries, Windows executables, macOS apps and more.

## Prerequisites
In order to develop Sphere (and do things such as building Sphere), you'll need the following installed:
* [Zapr](https://github.com/LiveG-Development/Zapr) (with Zapr added to your PATH)
* [Python 3](https://www.python.org/downloads) (with the `py` utility added to your PATH)
* [Node.js](https://nodejs.org/en/download) (with the `npm` utility added to your PATH)

## Building Sphere
To build and test Sphere, run at the command line in the project root directory if you're using Bash (for gDesk OS, Linux and macOS):

```bash
$ ./build.sh
```

Alternatively, run this in Command Prompt at the project root directory (for Windows):

```batch
build
```

This should then build Sphere by using Zapr, build the documentation files also by using Zapr and finally run Electron via npm. If you want to specify command-line arguments that Sphere should use when it runs, just append them to the end of the command.

## Available command-line arguments
Below is a list of command-line arguments that you can use with Sphere in order to take full control of it.

### `--debug`
```
--debug     Enter debug mode for Sphere.
```

Launch Chromium Dev Tools when Sphere runs (Sphere's debug mode) so that it can be debugged.

### `--help`
```
--help      Display this help screen.
```

Display the help screen that is a simpler equivalent to this section.

Aliases: `-h`, `/?`

### `--lang`
```
--lang      Force the UI language to be the locale specified.
            <locale>            The locale code to be used. For example, English (United Kingdom) would be `en_GB`.
```

Force the UI language to be the locale (in the format `xx_XX` where the first two letters are the language and the last two are the country) specified.

### `--mirroring-direction`
```
--mirroring-direction
            Force the UI text mirroring direction to be the direction specified.
            ltr                 Use the left-to-right (LTR) text mirroring direction.
            rtl                 Use the right-to-left (RTL) text mirroring direction.
```

Force the UI text mirroring direction to be the direction (either `ltr` for left-to-right mirroring or `rtl` for right-to-left mirroring) specified.