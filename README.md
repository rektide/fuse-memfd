# fuse-memfd

In memory filesystem backed by FUSE and Javascript and memfd_create

```
npm install -g fuse-memfd
```

## Usage

```
fuse-memfd ./mnt # mounts an in memory filesystem at ./mnt (needs to exists)
```

## Javascript API

You can access the FUSE operations from JS as well

```js
const Fuse = require('fuse-native')
const memfd = require('fuse-memfd')
const ops = memfd()

const fuse = new Fuse('./mnt', ops)
```

## License

MIT
