# vite-plugin-cross-origin-isolation

A vite plugin for enabling cross-origin-isolation for dev server.

`Cross origin isolation` is required for `SharedArrayBuffer`.

Using this plugin, in local dev server, functions that rely on SAB can be enabled and tested.

# Usage

`npm i -D vite-plugin-cross-origin-isolation`


In `vite.config.js`:
```
import crossOriginIsolation from 'vite-plugin-cross-origin-isolation'

export default {
    plugins: [
      // other plugins...
      crossOriginIsolation()
    ]
}
```