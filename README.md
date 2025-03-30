# LNReader Plugins

<p>
<img alt="LNReader plugins counting" src="https://raw.githubusercontent.com/LNReader/lnreader-plugins/plugins/v3.0.0/total.svg">
<img alt="GitHub issues by-label"  src="https://img.shields.io/github/issues/lnreader/lnreader-plugins/Source%20Request?color=success&label=source%20requests">
<img  alt="GitHub issues by-label"  src="https://img.shields.io/github/issues/lnreader/lnreader-plugins/Bug?color=red&label=bugs">
</p>

Repository to host plugins and related issues, and requests for
[LNReader](https://github.com/LNReader/lnreader).

## Installing

- Prerequisites: Nodejs >= 20

1. `npm install`

## Contributing

- [Quick start](./docs/quickstart.md)
- [Documentation](./docs/docs.md)

## Testing

#### via the testing website

1. Run `npm start` and open `localhost:3000` to test!

[Detailed tutorial for testing website](./docs/website-tutorial.md)

#### via an app

1. Plugins from GitHub
    * Run `npm run host-linux` or `npm run host-windows` (depending on your operating system)
    * Add your `https://raw.githubusercontent.com/<username>/<repo>/plugins/<tag>/.dist/plugins.min.json` to app repository
2. Plugins from localhost
    * Run `BASE_URL=<see below> npm run host-dev`
        * leave empty to use default: `https://raw.githubusercontent.com/${USERNAME}/${REPO}/${CURRENT_BRANCH}`
        * for android emulator use `http://10.0.2.2:3000`
        * for iOS simulator use `http://localhost:3000`
        * for a real device use the IP address of your computer in the local network (e.g. 192.168.21.37)
        * example for android emulator: `BASE_URL=http://10.0.2.2:3000 npm run host-dev`
    * Add plugin listing to app repository (e.g. for android emulator `http://10.0.2.2/.dist/plugins.min.json`)

---

The developer of this application does not have any affiliation with the content providers available.
