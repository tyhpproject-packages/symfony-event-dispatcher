<!-- tyhp-readme:start -->
# tyhpdef/symfony-event-dispatcher

Tyhp type definitions for `symfony/event-dispatcher` `7.4.17`.

```bash
composer require --dev tyhpdef/symfony-event-dispatcher:7.4.17
```

This is a metapackage. Composer also installs `tyhpdef/symfony-event-dispatcher-impl` (type files).
Require **this** name, not `tyhpdef/symfony-event-dispatcher-impl`.

See https://tyhplang.com.

## Maintain `symfony/event-dispatcher`? Ship the types yourself

If you are a Packagist maintainer of `symfony/event-dispatcher`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-event-dispatcher-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/event-dispatcher` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-event-dispatcher": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/event-dispatcher` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/event-dispatcher` with a real constraint,
   `"replace": { "tyhpdef/symfony-event-dispatcher": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/event-dispatcher` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-event-dispatcher` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
