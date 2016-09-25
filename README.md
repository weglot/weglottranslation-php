# Weglot PHP
The library to integrate Weglot translation to a PHP website


## Getting Started

### Install

Install the package via [Composer](https://getcomposer.org/doc/00-intro.md):

```bash
composer require "weglot/weglot-php":"dev-master"
```

If you don't use Composer, you can copy the `weglot.php` file and the `lib` directory to your project).

### Initialize
To initialize Weglot, you need your API Key. You can find it on [your Weglot account](https://weglot.com/account).

You need to enter Weglot initialization code at the beginning of the execution (Usually index.php or app.php)
```php
// composer autoload
require __DIR__ . '/vendor/autoload.php';
// if you are not using composer: require_once 'path/to/weglot.php';

$WG = new \Weglot\WG(array(
		"api_key" =>"YOUR API KEY",
		"original_l" =>"en", 
		"destination_l" =>"fr,de",
	));
```

### Check
flags
