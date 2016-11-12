## Getting Started

Follow these steps to run iChrome in Google Chrome as a developer.

- Open the url chrome://extensions/ in Google Chrome.
- Click to enable *Developer mode* so that you see developer options.
- Click the "Load unpackaged extensions..."
- Browse to the location where iChrome repo is installed, and select the sub-directory `naw-tab/app` as the extension source.
- When you make change to the code for the tab page, just reload the tab. (Yeah, this extension is written entirely with the good vanilla HTML/JS/CSS)

## gulp tasks

Those `babel` and `watch` tasks were not necessary anymore. I'm writting this extension in vanilla JS (with some advancement in ES6 syntax).

### Build and Package

[This section is not verified]

It will build your app as a result you can have a distribution version of the app in `dist`. Run this command to build your Chrome Extension app.

```bash
gulp build
```

You can also distribute your project with compressed file using the Chrome Developer Dashboard at Chrome Web Store. This command will compress your app built by `gulp build` command.

```bash
gulp package
```
