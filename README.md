# oxid_patches
How many times you have thought about OXID and "Do you want to ..." -> YES 
Don't do it again!

# first add this to your main composer file
composer require cweagans/composer-patches

# add this to your main composer file
    "extra": {
      "patches": {
        "oxid-esales/oxideshop-composer-plugin": {
          "don't copy module files to source, symlink it only":
          "https://git.d3data.de/D3Public/oxid_patches/raw/branch/symlinksInSource/symlinkmodules.patch"
        }
      },
      "enable-patching": true
    },

# run this command
composer install

Enjoy!
