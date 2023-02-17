# Installation

Add the repository to your `composer.json` file as shown below:

```json
{
  "repositories": [
    {
      "type": "package",
      "package": {
        "name": "yoerioptr/drupal_brecht",
        "version": "dev-main",
        "type": "drupal-module",
        "source": {
          "url": "https://github.com/yoerioptr/drupal_brecht.git",
          "type": "git",
          "reference": "main"
        }
      }
    }
  ]
}
```

Install the module using composer:

```bash
composer require yoerioptr/drupal_brecht:@dev
```