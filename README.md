# SNES-XDC

SNES-XDC is a Super Nintendo Entertainment System emulator packaged as a
[Webxdc](https://webxdc.org/) app. It runs the EmulatorJS SNES core locally
inside the app, with touch controls configured for mobile devices.

## Development

Requirements: Node.js and npm.

Install dependencies and start the Webxdc development server:

```sh
npm install
npm start
```

## Build

Create a `.xdc` app package in `dist/`:

```sh
npm run build
```

Each build increments the build number in `package.json` and updates
`version.js`; the resulting archive name uses that version.

## Game ROM

The app loads `game.sfc` from the project root. Replace that file with a ROM
you are legally permitted to use before building.

## Project files

- `index.html` configures the emulator and app display.
- `emulatorjs/data/` contains the locally bundled EmulatorJS runtime and
  emulator core assets.
- `manifest.toml` defines the Webxdc app metadata.
- `icon.png` is the app icon.
