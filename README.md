# Sylius Sitemap Bundle [![License](https://img.shields.io/packagist/l/stefandoorn/sylius-sitemap-bundle.svg)](https://packagist.org/packages/stefandoorn/sylius-sitemap-bundle) [![Version](https://img.shields.io/packagist/v/stefandoorn/sylius-sitemap-bundle.svg)](https://packagist.org/packages/stefandoorn/sylius-sitemap-bundle) [![Build status on Linux](https://img.shields.io/travis/stefandoorn/sylius-sitemap-bundle/master.svg)](http://travis-ci.org/stefandoorn/sylius-sitemap-bundle) [![Scrutinizer Quality Score](https://img.shields.io/scrutinizer/g/stefandoorn/sylius-sitemap-bundle.svg)](https://scrutinizer-ci.com/g/stefandoorn/sylius-sitemap-bundle/) [![Code Coverage](https://scrutinizer-ci.com/g/stefandoorn/sylius-sitemap-bundle/badges/coverage.png?b=master)](https://scrutinizer-ci.com/g/stefandoorn/sylius-sitemap-bundle/?branch=master)

## Big thanks

Goes out to the Sylius team. The core code of this bundle is created by the Sylius team.
Unfortunately it got removed from the Sylius core. Luckily the Sylius team approved the 
extraction to a separate bundle.

## Installation

1. Run `composer require stefandoorn/sylius-sitemap-bundle`.
2. Add to `app/AppKernel.php`:

```
  new SyliusSitemapBundle\SyliusSitemapBundle(),
```

3. Add to `app/config/config.yml`: 

```
  - { resource: "@SyliusSitemapBundle/Resources/config/config.yml" }
```

4. Add to `app/config/routing.yml`: 

```
sylius_sitemap:
     resource: "@SyliusSitemapBundle/Resources/config/routing.yml"
```