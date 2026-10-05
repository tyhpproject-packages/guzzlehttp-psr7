<!-- tyhp-readme:start -->
# tyhpdef/guzzlehttp-psr7

Tyhp type definitions for `guzzlehttp/psr7` `3.1.0`.

```bash
composer require --dev tyhpdef/guzzlehttp-psr7:3.1.0
```

This is a metapackage. Composer also installs `tyhpdef/guzzlehttp-psr7-impl` (type files).
Require **this** name, not `tyhpdef/guzzlehttp-psr7-impl`.

See https://tyhplang.com.

## Maintain `guzzlehttp/psr7`? Ship the types yourself

If you are a Packagist maintainer of `guzzlehttp/psr7`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/guzzlehttp-psr7-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `guzzlehttp/psr7` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/guzzlehttp-psr7": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `guzzlehttp/psr7` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `guzzlehttp/psr7` with a real constraint,
   `"replace": { "tyhpdef/guzzlehttp-psr7": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `guzzlehttp/psr7` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/guzzlehttp-psr7` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
