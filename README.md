# Modernizr Bundle for Symfony2

## Current Version

Modernizr 2.7.0
includes custom build similar to the one used by Zurb Foundation

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "bmatzner/modernizr-bundle": "~2.7"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Bmatzner\ModernizrBundle\BmatznerModernizrBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update bmatzner/modernizr-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
<script type="text/javascript" src="{{ asset('bundles/bmatznermodernizr/js/modernizr.min.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. http://modernizr.com
2. http://symfony.com
3. http://foundation.zurb.com
