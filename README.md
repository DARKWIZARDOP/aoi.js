  

# aoi.js
[![Discord Server](https://img.shields.io/discord/773352845738115102?color=5865F2&logo=discord&logoColor=white)](https://aoi.js.org/invite)
[![NPM Version](https://img.shields.io/npm/v/aoi.js.svg?maxAge=3600)](https://www.npmjs.com/package/aoi.js)
[![NPM Downloads](https://img.shields.io/npm/dt/aoi.js.svg?maxAge=3600)](https://www.npmjs.com/package/aoi.js)

## About
aoi.js is a package with customization and ready-to-use functions to make Discord Bots with ease.

- Interaction Commands Support
- Optimized and customizable 
- 500+ functions available  

The successor of [dbd.js](https://www.npmjs.com/package/dbd.js)

 
## Installation

**Node.JS 16.6.0 or newer is required.**  

```sh-session
npm install aoi.js
```

### Setting up

```js
const aoijs = require("aoi.js")

const bot = new aoijs.Bot({
token: "TOKEN",
prefix: "PREFIX",
intents: "all"
})

bot.onMessage() //Allows to execute Commands

bot.command({
name: "ping", //Trigger name (command name)
code: `Pong! $pingms` //Code inside of string
})

bot.readyCommand({
    channel: "", //Optional channnel ID
    code: `$log[Ready on $userTag[$clientID]]`
})
```

### Optional packages
- [tweetnacl](https://npmjs.com/tweetnacl) for music encryption (`npm install tweetnacl`)
- [@discordjs/opus](https://www.npmjs.com/package/@discordjs/opus) for encoding, primarily used for Music (`npm install @discordjs/opus`)
- [ffmpeg-static](https://www.npmjs.com/package/ffmpeg-static) for allowing Music Filters to run smoothly (`npm install ffmpeg-static`)
- [danbot-hosting](https://www.npmjs.com/package/danbot-hosting) for posting stats to their API (`npm install danbot-hosting`)


More Information in our [Documentation](https://aoi.leref.ga/guide/music)

## Links
- [Website](https://aoi.js.org)
- [Github](https://github.com/aoijs/aoi.js)
- [Discord Server](https://aoi.js.org/invite)
- [Documentation](https://aoi.leref.ga)

## Contributing
Please read [Contributing](https://github.com/aoijs/aoi.js/blob/main/.github/CONTRIBUTING.md)
