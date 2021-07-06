# arvis-google-translate
[![NPM](https://nodei.co/npm/arvis-google-translate.png)](https://nodei.co/npm/arvis-google-translate/)

### JetBrains' support

[![jetbrain](media/jetbrains.svg)](https://www.jetbrains.com/?from=arvis-google-translate)

## Installation

To use this workflow you must also install the [arvis-language-configuration](https://github.com/xfslove/arvis-language-configuration) workflow, and configure the language pair. See that [README](https://github.com/xfslove/arvis-language-configuration) for instructions.

* Voice feature not supported yet.

### With NPM
- Install with `npm install -g arvis-google-translate`.

## Usage

arvis workflow Keyword: `tr [word or sentence]`
Example: `tr kitchen sink` or `tr Hello, my name is arvis`

When translating a word you will see the translation as well as alternate translations if available.

With the first two results (which are the input word and the translation) you can…
- press <kbd>enter</kbd> to read the item.
- press <kbd>cmd</kbd>+<kbd>C</kbd> to copy the item.
- press <kbd>shift</kbd> open the translate website.
- press <kbd>cmd</kbd>+<kbd>L</kbd> to show the translation in large text.

The workflow will attempt to correct spelling mistakes which can be accepted with <kbd>enter</kbd>.

## 🔗 This workflow is converted from [alfred-workflow](https://github.com/xfslove/alfred-google-translate).

* Note that there might be some code change or different actions from the original workflow.

* Marked original workflow's creator to author.

## Environment Variables

| name       | default value                | description                                                  |
| ---------- | ---------------------------- | ------------------------------------------------------------ |
| domain     | https://translate.google.com | if you cannot access the default domain, you can config this. <br />大陆访问不了默认域名，所以如果使用2.x版本需要将这个变量设置为https://translate.google.cn. 或者还是使用[1.x版本](https://github.com/xfslove/arvis-google-translate/tree/v1.x) |
| voice      | remote                       | avaliable values: <br />remote: fetch voice from google, <br />local: use macOS local voice (notice: maybe only works on English),<br />none: dont use voice |
| save_count | 20                           | limit the translation history, see [arvis-translate-history](https://github.com/xfslove/arvis-translate-history).  <br />a value of 0 will keep no history |
| socks_proxy| -                            | not turned by default. you can specify local or remote socks proxy. format: `socks://{host}:{port}` example: local shadowsocks proxy 'socks://127.0.0.1:1086' |

##### 

## Screenshots

  ![](media/detect-lang.png)

  ![corrected.png](media/corrected.png)

- press <kbd>enter</kbd> to read or <kbd>cmd</kbd>+<kbd>C</kbd> to copy

    ![general.png](media/general.png)

- press <kbd>shift</kbd> to open the translation website

    ![quicklook.png](media/quicklook.png)

- press <kbd>cmd</kbd>+<kbd>L</kbd> to show the translation in large text [like this](#hotkey-and-largetype-snapshot).


## License

MIT © 
