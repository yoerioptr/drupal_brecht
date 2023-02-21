# Installation

Add the repository to your `composer.json` file as shown below:

```json
{
  "repositories": [
    {
      "type": "package",
      "package": {
        "name": "yoerioptr/drupal_brecht",
        "version": "dev-master",
        "type": "drupal-module",
        "source": {
          "url": "https://github.com/yoerioptr/drupal_brecht.git",
          "type": "git",
          "reference": "master"
        }
      }
    }
  ]
}
```

Add the following core patch:
```json
{
  "extra": {
    "patches": {
      "drupal/core": {
        "Add stream wrappers to access extension files": "https://www.drupal.org/files/issues/2021-12-15/1308152-395.patch"
      }
    }
  }
}
```

Install the module using composer:

```bash
composer require yoerioptr/drupal_brecht:@dev
```