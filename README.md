# session id patch

applicable for OXID 6.2 to 6.5.1

## first install the composer patch package
```
composer require cweagans/composer-patches
```

## add this to your main composer file
```
    "extra": {
      "patches": {
        "oxid-esales/oxideshop-ce": {
          "sessionid fix":
          "https://git.d3data.de/D3Public/oxid_patches/raw/branch/sessionid/sessionid.patch"
        }
      },
      "enable-patching": true
    },
```

## run this command
```
rm -rf ./vendor/oxid-esales/oxideshop-ce
composer install
```

Enjoy!
