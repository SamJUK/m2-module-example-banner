# SamJUK_ExampleBanner

Apart of a collection of modules, to help test/validate deployment processes.

Simple module that adds a banner below the page header when installed. With a feature flag in the system admin to toggle the output.

![Screenshot of the example banner](./example-banner.png)

## Installation
```sh
composer config repositories.samjuk-m2-module-example-banner vcs git@github.com:SamJUK/samjuk-m2-module-example-banner.git
composer require samjuk/m2-module-example-banner
php bin/magento cache:flush
```

## Feature Flag
The block output can be configured via a feature flag. This can be found in the admin panel under the `System Config > SamJUK > Example Banner > General > Enabled` path. Or set via the CLI with
```sh
php bin/magento config:set samjuk_examplebanner/general/enabled 0
php bin/magento cache:flush
```

## Related Modules

Name | Description | Link
--- | --- | ---
Example Footer | Adds 4 cta blocks to the top of the footer on all pages | https://github.com/SamJUK/m2-module-example-footer