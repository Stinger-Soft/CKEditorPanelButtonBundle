# CKEditor plugin Panel Button Bundle
Symfony2 Bundle to integrate the CKEditor plugin Panel Button

## Current Version

PanelButton v4.5.6

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/ckeditor-panelbutton-bundle": "~4.5.6"
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
        new Stinger\CKEditorPanelButtonBundle\StingerCKEditorPanelButtonBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/ckeditor-panelbutton-bundle
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

### Usage

``` yaml
trsteel_ckeditor:
    external_plugins:
      panelbutton:
        path: 'bundles/stingerckeditorpanelbutton'
```



# Licenses

Refer to the source code of the included files for license information

# References

1. http://ckeditor.com/addon/panelbutton
2. http://symfony.com
 