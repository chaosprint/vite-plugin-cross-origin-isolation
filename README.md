# vite-plugin-cross-origin-isolation

A vite plugin for enabling cross-origin-isolation for dev server.


## Why

`Cross origin isolation` is required for `SharedArrayBuffer`.

Using this plugin, in local dev server, functions that rely on SAB can be enabled and tested.

## Usage

First install it in your vite project:

`npm i -D vite-plugin-cross-origin-isolation`

Then, in `vite.config.js`:

```
import crossOriginIsolation from 'vite-plugin-cross-origin-isolation'

export default {
    plugins: [
      // other plugins...
      crossOriginIsolation()
    ]
}
```

## License
The MIT License (MIT)

Copyright (c) 2021 - present Qichao Lan (chaosprint)
