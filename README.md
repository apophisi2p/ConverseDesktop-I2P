# Converse Desktop

## Jabber/XMPP client based on Converse.js and Electron


A basic integration of Converse.js `https://conversejs.org/` and Electron. With OMEMO.

- Tray icon
- Tray notifications
- All the best from Converse.js like system notifications, MAM, OMEMO etc. 



## Build from source

```bash
git clone http://git.apophis.i2p/apophis/ConverseDesktop-I2P.git
cd ConverseDesktop-I2P
npm i
$(npm bin)/electron-rebuild
```

Then, to run:

```bash
npm start
```

### Build targets:

| Operation System | Target                 |
|------------------|------------------------|
| macOS            | `npm run dist`         |
| Windows          | `npm run dist:win64`   |
| Linux            | `npm run dist:linux64` |

More targets could be added via `package.json`. 


## License

Like Converse.js, Converse Desktop's files are released under the Mozilla Public License version 2 (MPLv2). The gist of this license is that the covered files must stay open source, and modifications to them need to be released under the same license, but new files (for example for your own plugin) don't have to be released under the same license.

However, libsignal library, which is required for OMEMO support is released under the GPLv3. The MPLv2 license is compatible with GPLv3 and when GPLv3 code is included, the entire project effectively is licensed under the GPLv3.

Any custom build of Converse Desktop without libsignal included will again be licensed
under the MPLv2.


## Acknowledgements

This project started as a fork of Nick Denry's Chimeverse `https://github.com/conversejs/converse-desktop`.

