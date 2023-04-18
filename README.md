# @webcatalog-oss/electron-settings

> A fork of [electron-settings](https://github.com/nathanbuchar/electron-settings) from [WebCatalog](https://about.webcatalog.io/) with active maintenance & enhancements.

A simple and robust settings management library for [Electron](https://electronjs.org).

Born from Atom's original internal configuration manager and the settings manager of choice for Electron's own [API Demos app](https://github.com/electron/electron-api-demos), Electron Settings allows you to persist user settings and other data between app loads simply and easily.

### Install

```
npm install @webcatalog-oss/electron-settings
```

### Demo

```ts
import settings from 'electron-settings';

await settings.set('color', {
  name: 'cerulean',
  code: {
    rgb: [0, 179, 230],
    hex: '#003BE6'
  }
});

await settings.get('color.name');
// => "cerulean"

await settings.get('color.code.rgb[1]');
// => 179
```

### API Docs

API docs and can be found at [https://webcatalog.github.io/electron-settings/](https://webcatalog.github.io/electron-settings/).
