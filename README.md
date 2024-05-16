# Patches for [Litefyr]

Sometimes there are [composer] [packages] who need a patch in order to work correctly with [Neos]. In order to have a
central place to manage them, we've created this repository. You can either download the patches and include it into
your Distribution or you can also include it directly. In order to do this, make sure this settings is in your root
`composer.json`:

```json
{
    "extra": {
        "patches-file": "https://raw.githubusercontent.com/Litefyr/Patches/main/patches.json"
    }
}
```

Also you need to make sure that [`cweagans/composer-patches`] is installed and set up under [`config.allow-plugins`]
correctly

```json
{
    "config": {
        "allow-plugins": {
            "cweagans/composer-patches": true
        }
    }
}
```

[Litefyr]: https://litefyr.io
[neos]: https://neos.io
[composer]: https://getcomposer.org
[packages]: https://packagist.org
[`cweagans/composer-patches`]: https://packagist.org/packages/cweagans/composer-patches
[`config.allow-plugins`]: https://getcomposer.org/doc/06-config.md#allow-plugins
