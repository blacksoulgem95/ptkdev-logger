[![Beautiful Node Logger: the best alternative to the console.log statement](https://raw.githubusercontent.com/ptkdev/ptkdev-logger/nightly/.github/assets/ptkdev-logger-logo.png)](https://www.npmjs.com/package/@ptkdev/logger)

# 🦒 Beautiful Node Logger

[![](https://img.shields.io/badge/version-v1.0.0-lightgrey.svg)](https://github.com/ptkdev/ptkdev-logger/releases) [![](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://github.com/ptkdev/ptkdev-logger/blob/master/LICENSE.md) [![](https://img.shields.io/badge/ES-9-F7DF1E.svg)](https://wikipedia.org/wiki/ECMAScript) [![](https://snyk.io/test/github/ptkdev/ptkdev-logger/badge.svg)](https://snyk.io/test/github/ptkdev/ptkdev-logger) [![](https://discordapp.com/api/guilds/383373985666301975/embed.png)](http://discord.ptkdev.io)

> The best alternative to the console.log statement

## 🎁 Support: Donate
> This project is **free**, **open source** and I try to provide excellent **free support**. Why donate? I work on this project several hours in my spare time and try to keep it up to date and working. **THANK YOU!**

[![](https://img.shields.io/badge/donate-paypal-005EA6.svg?logo=paypal)](https://www.paypal.me/ptkdev) [![](https://img.shields.io/badge/donate-patreon-F87668.svg?logo=patreon)](https://www.patreon.com/ptkdev) [![](https://img.shields.io/badge/donate-sponsors-ea4aaa.svg?logo=github)](https://github.com/sponsors/ptkdev/)  [![](https://img.shields.io/badge/donate-ko--fi-29abe0.svg?logo=ko-fi)](https://ko-fi.com/ptkdev)

![](https://img.shields.io/badge/bitcoin-35jQmZCy4nsxoMM3QPFrnZePDVhdKaHMRH-E38B29.svg?logo=bitcoin) ![](https://img.shields.io/badge/ethereum-0x8b8171661bEb032828e82baBb0B5B98Ba8fBEBFc-4E8EE9.svg?logo=ethereum)

## 📎 Menu
- 💡 [Features](#-features)
- 👔 [Screenshot](#-screenshot)
- 🚀 [How to use](#-installation)
- 📚 [Documentation](#-documentation)
- ❤️ [Contributing](#-contributing)
- 🐛 [Known Bugs](https://github.com/ptkdev/ptkdev-logger/issues?q=is%3Aopen+is%3Aissue+label%3Abug)
- 🍻 Community:
  - <img src="https://raw.githubusercontent.com/ptkdev/ptkdev-logger/master/.github/assets/social_discord.png" height="18px"> [Discord](http://discord.ptkdev.io) ([🇬🇧 English Channel](https://discord.gg/tWtqt4B) | [🇮🇹 Italian Channel](https://discord.gg/q29uZnm) | [🇵🇱 Polish Channel](https://discord.gg/akjuWJX))

## 💡 Features
* [✔️] Easy to use
* [✔️] MIT License
* [✔️] The best alternative to the console.log statement
* [✔️] Translations: 🇬🇧 🇮🇹 🇵🇱 (Help me ❤️)

## 👔 Screenshot
[![Beautiful Node Logger](https://raw.githubusercontent.com/ptkdev/ptkdev-logger/nightly/.github/assets/screenshot/ptkdev-logger-screen1.png)](https://raw.githubusercontent.com/ptkdev/ptkdev-logger/nightly/.github/assets/screenshot/ptkdev-logger-screen1.png)

## 🚀 Installation
1. In your node project run: `npm install @ptkdev/logger --save`
2. Usage:
```javascript
const Logger = require("@ptkdev/logger");
const logger = new Logger();
logger.info("message");
```

You can set `options` to `new Logger(options);` example:
```javascript
const Logger = require("@ptkdev/logger");

const options = {
	"language": "en",
	"colors": true,
	"debug": true,
	"info": true,
	"warning": true,
	"errors": true,
	"sponsor": true,
	"write": true,
	"path": {
		"debug_log": "./debug.log",
		"error_log": "./errors.log",
	}
};

const logger = new Logger(options);
logger.info("message");
```

See folder `examples`, run with `node example.js`. Below is available a description of `options` values and all logger methods.

## Options

| Parameter | Description | Values | Default value |
| --- | --- | --- | --- |
| language | Set language of log type | en\|it\|pl | en |
| colors | Enable colors in terminal | true\|enabled\|false\|disabled | true |
| debug | Enable all logs with method debug | true\|enabled\|false\|disabled | true |
| info | Enable all logs with method info | true\|enabled\|false\|disabled | true |
| warning | Enable all logs with method warning | true\|enabled\|false\|disabled | true |
| errors | Enable all logs with method errors | true\|enabled\|false\|disabled | true |
| sponsor | Enable all logs with method sponsor | true\|enabled\|false\|disabled | true |
| write |  Write the logs into a file, you need set path values | true\|enabled\|false\|disabled | false |
| path | If write is true, the library writes the logs to a path | Object | `{"debug_log": "./debug.log", "error_log": "./errors.log"}` |

## Methods

| Method | Description | Parameters |
| --- | --- | --- |
| debug(__message__, __tag__) | `message`: Display debug log message <br> `tag`: prefix of message | `message`: string (mandatory) <br> `tag`: string (optional) |
| info(__message__, __tag__) | `message`: Display info log message <br> `tag`: prefix of message | `message`: string (mandatory) <br> `tag`: string (optional) |
| warning(__message__, __tag__) | `message`: Display warning log message <br> `tag`: prefix of message | `message`: string (mandatory) <br> `tag`: string (optional) |
| errors(__message__, __tag__) | `message`: Display errors log message <br> `tag`: prefix of message | `message`: string (mandatory) <br> `tag`: string (optional) |
| sponsor(__message__, __tag__) | `message`: Display sponsor log message <br> `tag`: prefix of message | `message`: string (mandatory) <br> `tag`: string (optional) |
| stackoverflow(__message__, __tag__, __error_string__) | `message`: Display stackoverflow log message <br> `tag`: prefix of message <br> `error_string`: query for stackoverflow, if empty we use message param | `message`: string (mandatory) <br> `tag`: string (optional) <br> `error_string`: string (optional) |
| docs(__message__, __url__, __tag__,) | `message`: Display docs log message <br> `url`: link of documentation <br> `tag`: prefix of message | `message`: string (mandatory) <br> `url`: string (optional) <br> `tag`: string (optional) |

## 📚 Documentation
Run `npm run docs`

## 👑 Sponsors
Support this project by becoming a sponsor. 🙏 Become a sponsor on [patreon](https://www.patreon.com/join/ptkdev) or become top3 sponsor on [ko-fi](https://ko-fi.com/ptkdev). Your logo will show up here with a link to your website.

[![](https://api.ptkdev.io/backers/sponsor1.png)](https://api.ptkdev.io/backers/sponsor1.html) [![](https://api.ptkdev.io/backers/sponsor2.png)](https://api.ptkdev.io/backers/sponsor2.html) [![](https://api.ptkdev.io/backers/sponsor-kofi1.png)](https://api.ptkdev.io/backers/sponsor-kofi1.html) [![](https://api.ptkdev.io/backers/sponsor-kofi2.png)](https://api.ptkdev.io/backers/sponsor-kofi2.html) [![](https://api.ptkdev.io/backers/sponsor-kofi3.png)](https://api.ptkdev.io/backers/sponsor-kofi3.html) [![](https://api.ptkdev.io/backers/sponsor3.png)](https://api.ptkdev.io/backers/sponsor3.html) [![](https://api.ptkdev.io/backers/sponsor4.png)](https://api.ptkdev.io/backers/sponsor4.html) [![](https://api.ptkdev.io/backers/sponsor5.png)](https://api.ptkdev.io/backers/sponsor5.html) [![](https://api.ptkdev.io/backers/sponsor6.png)](https://api.ptkdev.io/backers/sponsor6.html) [![](https://api.ptkdev.io/backers/sponsor7.png)](https://api.ptkdev.io/backers/sponsor7.html) [![](https://api.ptkdev.io/backers/sponsor8.png)](https://api.ptkdev.io/backers/sponsor8.html) [![](https://api.ptkdev.io/backers/sponsor9.png)](https://api.ptkdev.io/backers/sponsor9.html) [![](https://api.ptkdev.io/backers/sponsor10.png)](https://api.ptkdev.io/backers/sponsor10.html) [![](https://api.ptkdev.io/backers/sponsor11.png)](https://api.ptkdev.io/backers/sponsor11.html) [![](https://api.ptkdev.io/backers/sponsor12.png)](https://api.ptkdev.io/backers/sponsor12.html) [![](https://api.ptkdev.io/backers/sponsor13.png)](https://api.ptkdev.io/backers/sponsor13.html) [![](https://api.ptkdev.io/backers/sponsor14.png)](https://api.ptkdev.io/backers/sponsor14.html) [![](https://api.ptkdev.io/backers/sponsor15.png)](https://api.ptkdev.io/backers/sponsor15.html)

## 🦄 Backers
Thank you to all our backers! 🙏 Become a backer on [patreon](https://www.patreon.com/join/ptkdev).

[![](https://api.ptkdev.io/backers/backer1.png)](https://api.ptkdev.io/backers/backer1.html) [![](https://api.ptkdev.io/backers/backer2.png)](https://api.ptkdev.io/backers/backer2.html) [![](https://api.ptkdev.io/backers/backer3.png)](https://api.ptkdev.io/backers/backer3.html) [![](https://api.ptkdev.io/backers/backer4.png)](https://api.ptkdev.io/backers/backer4.html) [![](https://api.ptkdev.io/backers/backer5.png)](https://api.ptkdev.io/backers/backer5.html) [![](https://api.ptkdev.io/backers/backer6.png)](https://api.ptkdev.io/backers/backer6.html) [![](https://api.ptkdev.io/backers/backer7.png)](https://api.ptkdev.io/backers/backer7.html) [![](https://api.ptkdev.io/backers/backer8.png)](https://api.ptkdev.io/backers/backer8.html) [![](https://api.ptkdev.io/backers/backer9.png)](https://api.ptkdev.io/backers/backer9.html) [![](https://api.ptkdev.io/backers/backer10.png)](https://api.ptkdev.io/backers/backer10.html) [![](https://api.ptkdev.io/backers/backer11.png)](https://api.ptkdev.io/backers/backer11.html) [![](https://api.ptkdev.io/backers/backer12.png)](https://api.ptkdev.io/backers/backer12.html) [![](https://api.ptkdev.io/backers/backer13.png)](https://api.ptkdev.io/backers/backer13.html) [![](https://api.ptkdev.io/backers/backer14.png)](https://api.ptkdev.io/backers/backer14.html) [![](https://api.ptkdev.io/backers/backer15.png)](https://api.ptkdev.io/backers/backer15.html)

## ❤️ Contributing
I 💟 contributions! I will happily accept your pull request! Translations, grammatical corrections (GrammarNazi you are welcome! Yes my English is bad, sorry), etc... Do not be afraid, if the code is not perfect we will work together 👯 and remember to insert your name in `.all-contributorsrc` and `package.json` file.

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://ptk.dev"><img src="https://avatars1.githubusercontent.com/u/442844?v=4" width="100px;" alt=""/><br /><sub><b>Patryk Rzucidło</b></sub></a><br /><a href="https://github.com/ptkdev/ptkdev-logger/commits?author=ptkdev" title="Code">💻</a> <a href="#translation-ptkdev" title="Translation">🌍</a> <a href="https://github.com/ptkdev/ptkdev-logger/commits?author=ptkdev" title="Documentation">📖</a> <a href="https://github.com/ptkdev/ptkdev-logger/issues?q=author%3Aptkdev" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/agoalofalife"><img src="https://avatars1.githubusercontent.com/u/15719824?v=4" width="100px;" alt=""/><br /><sub><b>Ilua Chubarov</b></sub></a><br /><a href="https://github.com/ptkdev/ptkdev-logger/commits?author=agoalofalife" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

> 💰 In the future, if the donations allow it, I would like to share some of the success with those who helped me the most. For me open source is share of code, share development knowledges and share donations!

## 📲 Tools
[![](https://img.shields.io/badge/portfolio-ptkdev-000000.svg)](https://ptk.dev/)
[![](https://img.shields.io/badge/app-meingifs-E1215B.svg)](https://meingifs.pics/)
[![](https://img.shields.io/badge/stickers-ptkdev-128C7E.svg)](https://stickers.ptkdev.io/)

[![](https://img.shields.io/badge/app-social%20manager%20tools-ff7f19.svg)](http://logger.ptkdev.io/)
[![](https://img.shields.io/badge/api-instagram%20bot-895a4d.svg)](https://github.com/ptkdev/ptkdev-logger)
[![](https://img.shields.io/badge/api-twitter%20bot-21B7F4.svg)](https://github.com/social-manager-tools/socialmanagertools-twbot)
[![](https://img.shields.io/badge/api-facebook%20bot-3b5998.svg)](https://github.com/social-manager-tools/socialmanagertools-fbbot)
[![](https://img.shields.io/badge/telegram%20bot-feed%20rss%20for%20wordpress%20&amp;%20medium-00AB6C.svg)](https://github.com/social-manager-tools/socialmanagertools-tgbot)

## 🐍 Sorry for snake_case
I love snake_case syntax sorry for this 😭 don't hate me.

## 💫 License
* Code and Contributions have **MIT License**
* Images and logos have **CC BY-NC 4.0 License** ([Freepik](https://it.freepik.com/) Premium License)
* Documentations and Translations have **CC BY 4.0 License**

###### Copyleft (c) 2020 [Patryk Rzucidło](https://ptk.dev) ([@PTKDev](https://twitter.com/ptkdev)) <[support@ptkdev.io](mailto:support@ptkdev.io)>