![Global Twitch Emotes banner](/marquee.png)

A browser extension which replaces all Twitch.tv emote phrases with their actual emoticons.

Currently supports Chrome, Firefox, and Opera. Edge support is planned, Safari support is not.

##  Building

Global Twitch Emotes is built using Node.js. Download and install the latest version of Node.js [here](https://nodejs.org/).

1.  Navigate to the parent directory.
2.  Run ```npm install```
3.  Then run <pre>npm run-script build <b>VERSION BROWSER</b></pre> 

    **VERSION:** Extension version to build.

    `test` | `release`
    
    *Release builds are minified, stripped of all `console` calls, and zipped into a .zip file for distribution, whilst test builds are not minified, to allow for easier debugging.*
    
    **BROWSER:** The browser type you want to build for.

    `webkit` | `firefox` | `edge`
    
    | **Parameter** | **Applicable Browser(s)**                         |
    |---------------|---------------------------------------------------|
    | webkit        | Chromium-based browsers (Chrome, Opera, etc.)     |
    | firefox       | Firefox                                           |
    | edge          | Edge                                              |
    
    *The script will build for all browser types if the browser parameter is not specified.*

##  Installation

Built extensions can be found in the newly-generated `build` directory. You can side-load the unpacked extension in order to run it in your browser. Please refer to your browser's extension installation guide for details.

##  Testing

In the parent directory, run `npm run-script test` to run all test files found in the `test` directory.
    
##  Support

For inquiries, please either [contact me](mailto:mohamed.y.elalawi@gmail.com) or [open an issue](https://github.com/melalawi/GlobalTwitchEmotes/issues/new).
