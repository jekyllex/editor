# JekyllEx Editor

This is a lightweight web-based code editor designed to enhance the file editing experience on the [JekyllEx](https://jekyllex.xyz) android app.

The editor is embedded in the app with a native JavaScript bridge to allow communication - loading files into the editor and saving edits back to the file system.

It uses a [forked variant](https://github.com/jekyllex/editor/tree/main/assets/js/prism-live) of the [Prism.js Live](https://github.com/PrismJS/live) beta library & a few plugins to provide:

- Usable real-time syntax highlighting.
- Multiple customizable themes.
- Debounced saving, with the option to control timeouts.
- Lazy loading of language sets to enhance markdown code blocks editing.

The editor supports the following query params:

- `theme`: The ID (`0` through `7`) of the theme to load in the editor. Defaults to `0`.
- `timeout`: The time in milliseconds to wait before calling the `IOBridge` callback that saves text. Defaults to `1000`.
- `lang`: The shortname of the default language to be used for syntax highlighting. Defaults to `rb`. For jekyll flavored markdown, use `md`.

## Previews

The editor supports the following themes:

| <img src="https://raw.githubusercontent.com/jekyllex/editor/main/assets/previews/one-light.webp" alt="One Light" width="300" /> <br> <p align="center">**One Light**</p> | <img src="https://raw.githubusercontent.com/jekyllex/editor/main/assets/previews/one-dark.webp" alt="One Dark" width="300" /> <br> <p align="center">**One Dark**</p> |
| ------------------------------------------------------------- | ------------------------------------------------------------- |
| <img src="https://raw.githubusercontent.com/jekyllex/editor/main/assets/previews/duotone-dark.webp" alt="Duotone Dark" width="300" /> <br> <p align="center">**Duotone Dark**</p> | <img src="https://raw.githubusercontent.com/jekyllex/editor/main/assets/previews/duotone-space.webp" alt="Duotone Space" width="300" /> <br> <p align="center">**Duotone Space**</p> |
| <img src="https://raw.githubusercontent.com/jekyllex/editor/main/assets/previews/coldark-cold.webp" alt="Coldark Cold" width="300" /> <br> <p align="center">**Coldark Cold**</p> | <img src="https://raw.githubusercontent.com/jekyllex/editor/main/assets/previews/coldark-dark.webp" alt="Coldark Dark" width="300" /> <br> <p align="center">**Coldark Dark**</p> |
| <img src="https://raw.githubusercontent.com/jekyllex/editor/main/assets/previews/solarized-light.webp" alt="Solarized Light" width="300" /> <br> <p align="center">**Solarized Light**</p> | <img src="https://raw.githubusercontent.com/jekyllex/editor/main/assets/previews/tomorrow-night.webp" alt="Tomorrow Night" width="300" /> <br> <p align="center">**Tomorrow Night**</p> |


## License

This project is [`MIT`](https://github.com/jekyllex/editor/blob/main/LICENSE) licensed.

```
MIT License

Copyright (c) 2021 Prism Live
Copyright (c) 2024 Gourav Khunger

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
