# Whoops service provider for Silex

## Installation

In your silex app root:

```
composer require nassau/silex-whoops@dev-master
```

And then register it in your code:

```
/** @var \Pimple\Container $app */
$app->register(new \Nassau\SilexWhoops\WhoopsServiceProvider);
```

It requires `silex/silex:~2.0@dev`. For silex version ~1.0 the service provider is bundled with `filp/whoops` package.

## Configuration

Define your own handler by overriding the `whoops.error_page_handler` key in the container.

See also: [filp/whoops](https://github.com/filp/whoops)
