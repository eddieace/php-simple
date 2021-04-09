php-simple
==========================

Version 1.0.4

PSR-4 compatible

Updated version of the simplehtmldom for php 7.3+.

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
use Eddieace\PhpSimple\HtmlDomParser;

...
$dom = HtmlDomParser::str_get_html( $str );
or 
$dom = HtmlDomParser::file_get_html( $file_name );

$elems = $dom->find($elem_name);
...
```
Example
-----
```php
use Eddieace\PhpSimple\HtmlDomParser;

$html = HtmlDomParser::file_get_html("http://example.com/");
$results = $html->find('h1');
echo $results[0]->plaintext;

//output : Example Domain

```
