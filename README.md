Bootstrap Bundle for Symfony2
=======================

## Current Version

Bootstrap.js 3.3.6

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "alexandermatveev/bootstrap-bundle": "*"
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
        new AlexanderMatveev\BootstrapBundle\AlexanderMatveevBootstrapBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update alexandermatveev/bootstrap-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ bin/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ bin/console assets:install --symlink web
```

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
<link href="{{ asset('bundles/alexandermatveevbootstrap/js/bootstrap/css/bootstrap.min.css') }}" rel="stylesheet">
<script type="text/javascript" src="{{ asset('bundles/alexandermatveevbootstrap/js/bootstrap/js/bootstrap.min.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. http://getbootstrap.com/
2. http://symfony.com
