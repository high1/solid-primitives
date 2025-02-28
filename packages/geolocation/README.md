# @solid-primitives/geolocation

[![lerna](https://img.shields.io/badge/maintained%20with-lerna-cc00ff.svg)](https://lerna.js.org/)

Primitives to query and watch geolocation information.

`createGeolocation` - Used to fetch current geolocation data as a resource.

`createGeolocationWatcher` - Creates a geolocation watcher and updates a signal with the latest coordinates.

## How to use it

Basic use with refetch:

```ts
const [location, refetch] = createGeolocation();
```

or with options:

```ts
const [location, refetch] = createGeolocation({
  enableHighAccuracy: false,
  maximumAge: 0,
  timeout: 200
});
```

or to watch geolocation:

```ts
const [location, error] = createGeolocationWatcher(true);
```

## Demo

You may view a working example here: https://codesandbox.io/s/solid-primitives-geolocation-fhzu4?file=/src/index.tsx

## Changelog

<details>
<summary><b>Expand Changelog</b></summary>

0.0.100

Pulling an early release of the package together and preparing for 1.0.0 release. No changes.

1.0.0

Added testing, improved types, changed name of createGeolocationWatcher to createGeolocationMonitor.

</details>
