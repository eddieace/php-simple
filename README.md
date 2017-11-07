php-simple
==========================

Version 1.0.0

Adaptation for Composer and PSR-0 of:

Updated version of the simplehtmldom for php 7.1+.

http://simplehtmldom.sourceforge.net/

Install
-------

 composer.phar
```json
"require": {
    "eddieace/php-simple": "1.0.*"
    }
```
 composer require
```json
	composer require eddieace/php-simple
```

Usage
-----

```php
use Eddieace\PhpSimple\;

...
$dom = HtmlDomParser::str_get_html( $str );
or 
$dom = HtmlDomParser::file_get_html( $file_name );

$elems = $dom->find($elem_name);
...

```