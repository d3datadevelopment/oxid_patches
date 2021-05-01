# oxid_patches
permission error while deleting the generated unified namespace helper in vagrant shared folder when running unit tests

# first add this to your main composer file
composer require cweagans/composer-patches

# add this to your main composer file
    "extra": {
      "patches": {
        "oxid-esales/testing-library": {
          "unifiled issues in vagrant":
          "https://git.d3data.de/D3Public/oxid_patches/raw/branch/unifiedIssuesInVagrant/unifiedIssuesInVagrant.patch"
        }
      },
      "enable-patching": true
    },

# run this command
composer install

Enjoy!
