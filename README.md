# Laravel Response Macros

[![Latest Version on Packagist](https://img.shields.io/packagist/v/appstract/laravel-response-macros.svg?style=flat-square)](https://packagist.org/packages/appstract/laravel-response-macros)
[![Total Downloads](https://img.shields.io/packagist/dt/appstract/laravel-response-macros.svg?style=flat-square)](https://packagist.org/packages/appstract/laravel-response-macros)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Build Status](https://img.shields.io/travis/appstract/:package_name/master.svg?style=flat-square)](https://travis-ci.org/appstract/laravel-response-macros)

This package is a collection of custom response macros that you can re-use in a variety of your routes and controllers.

## Installation

You can install the package via composer:

``` bash
composer require appstract/laravel-response-macros
```

### Provider

Then add the ServiceProvider to your `config/app.php` file:

```
'providers' => [
    ...

    Appstract\ResponseMacros\ResponseMacrosServiceProvider::class,

    ...
]
```

## Usage

``` php
return response()->message('hello world!', 200);
```

## Result

``` json
{
    "message": "hello world!",
    "status": 200
}
```

## Testing

``` bash
$ composer test
```

## Contributing

Contributions are welcome, [thanks to y'all](https://github.com/appstract/laravel-blade-directives/graphs/contributors) :)

## About Appstract

Appstract is a small team from The Netherlands. We create (open source) tools for webdevelopment and write about related subjects on [Medium](https://medium.com/appstract). You can [follow us on Twitter](https://twitter.com/teamappstract), [buy us a beer](https://www.paypal.me/teamappstract/10) or [support us on Patreon](https://www.patreon.com/appstract).

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
