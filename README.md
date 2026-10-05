<!-- tyhp-readme:start -->
# tyhpdef/pda-pheanstalk

Tyhp type definitions for `pda/pheanstalk` `8.0.2`.

```bash
composer require --dev tyhpdef/pda-pheanstalk:8.0.2
```

This is a metapackage. Composer also installs `tyhpdef/pda-pheanstalk-impl` (type files).
Require **this** name, not `tyhpdef/pda-pheanstalk-impl`.

See https://tyhplang.com.

## Maintain `pda/pheanstalk`? Ship the types yourself

If you are a Packagist maintainer of `pda/pheanstalk`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/pda-pheanstalk-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `pda/pheanstalk` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/pda-pheanstalk": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `pda/pheanstalk` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `pda/pheanstalk` with a real constraint,
   `"replace": { "tyhpdef/pda-pheanstalk": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `pda/pheanstalk` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/pda-pheanstalk` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
