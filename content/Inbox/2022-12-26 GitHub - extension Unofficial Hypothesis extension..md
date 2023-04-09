---
title: "2022-12-26 GitHub - Unofficial Hypothesis extension."
---

[[- ReadItLater]] [[- Article]] [[- InternetScrap]]

# [GitHub - diegodlh/unofficial-hypothesis-extension: Unofficial Hypothesis extension.](https://github.com/diegodlh/unofficial-hypothesis-extension)

## Unofficial Hypothesis extension

[![BSD licensed](https://camo.githubusercontent.com/44c92aa855b3a4b0b5c6f84818afb96ab66b53a102115f5167a396a3f0ff8f3a/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6c6963656e73652d4253442d626c75652e737667)](https://github.com/diegodlh/unofficial-hypothesis-extension/blob/master/LICENSE)

The *unofficial* Hypothesis extension allows you to annotate web documents using your [Hypothesis](https://hypothes.is/) account.

It is a fork of the *official* [Hypothesis browser extension(s)](https://github.com/hypothesis/browser-extension). Its main purpose is to provide a working extension for the Firefox browser. See this [thread](https://github.com/hypothesis/browser-extension/issues/310) for more details.

To install on your Firefox browser, download it from [here](https://addons.mozilla.org/en-US/firefox/addon/unofficial-hypothesis/).

[![Screenshot of Hypothesis client](Screenshot%20of%20Hypothesis%20client.png)](https://github.com/diegodlh/unofficial-hypothesis-extension/blob/master/images/screenshot.png?raw=true)

## Extra features

As of v1.470.0.1, the Unofficial extension for Hypothesis enables some customization of the annotation client. Read more about it [here](https://github.com/diegodlh/unofficial-hypothesis-extension/blob/master/docs/extra-features.md).

## Known bugs

-   Annotating local PDFs is not supported because Firefox is more restrictive than Chrome regarding extension access to local files. See issue [#100](https://github.com/hypothesis/browser-extension/issues/100).

## Contribute

**Do you like this extension?**

Please, star it here and review it on [AMO](https://addons.mozilla.org/en-US/firefox/addon/unofficial-hypothesis/).

**Would you like to support its development and maintenance?**

[Buy me](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=Z96DVUZGG3ZKU&source=url) a coffee, or a beer ;)

**Did you find a bug?**

Please, report it [here](https://github.com/diegodlh/unofficial-hypothesis-extension/issues)!

**Do you have suggestions, or ideas for new features?**

I’ll be happy to hear about them! Let’s discuss them [here](https://github.com/diegodlh/unofficial-hypothesis-extension/issues).

## Development

The code for the extensions is in the `src/` directory, and can be built into a browser extension by running:

```
npm install
make SETTINGS_FILE=settings/firefox-prod-amo.json
```

Once this is done you should be able to load the `build/` directory as an unpacked extension.

Use `settings/firefox-prod-self.json` for self distribution, instead of distribution through AMO (addons.mozilla.org). This includes the update\_url field in the manifest.json file to handle automatic updates of the self distributed extension.

The extension code has a test suite, which you can run using:

Note that the browser extensions are for the most part just a wrapper around the [*unofficial* Hypothesis client](https://github.com/diegodlh/unofficial-hypothesis-client/). Depending on what you're interested in working on, you may need to check out the client repository too. If you do that, you can get the browser extension repository to use your checked-out `unofficial-hypothesis-client` repository by running

in the `unofficial-hypothesis-client` repository, and then

```
npm link unofficial-hypothesis
```

in the `unofficial-browser-extension` repository. After that, a call to `make` will use the built client from the client repository. Please consult the client's documentation for instructions on building the client in a development environment.

**Tip**: If you get a **permission denied** error when running `npm link` you probably need to fix npm's permissions. See [Fixing npm permissions](https://docs.npmjs.com/getting-started/fixing-npm-permissions).

**Tip**: To **unlink** your dev browser extension from your dev client run `npm unlink unofficial-hypothesis` in your browser extension directory (see the [npm uninstall docs](https://docs.npmjs.com/cli/uninstall)).

See [Building the extension](https://github.com/diegodlh/unofficial-hypothesis-extension/blob/master/docs/building.md) for more information.

## License

The *unofficial* Hypothesis extension is released under the [2-Clause BSD License](http://www.opensource.org/licenses/BSD-2-Clause), sometimes referred to as the "Simplified BSD License". Some third-party components are included. They are subject to their own licenses. All of the license information can be found in the included [LICENSE](https://github.com/diegodlh/unofficial-hypothesis-extension/blob/master/LICENSE) file.