# Which
A PHP library for locating commands in a PATH.

[![Build Status](http://img.shields.io/travis/nubs/which.svg?style=flat)](https://travis-ci.org/nubs/which)
[![Scrutinizer Code Quality](http://img.shields.io/scrutinizer/g/nubs/which.svg?style=flat)](https://scrutinizer-ci.com/g/nubs/which/)
[![Code Coverage](http://img.shields.io/scrutinizer/coverage/g/nubs/which.svg?style=flat)](https://scrutinizer-ci.com/g/nubs/which/)

[![Latest Stable Version](http://img.shields.io/packagist/v/nubs/which.svg?style=flat)](https://packagist.org/packages/nubs/which)
[![Total Downloads](http://img.shields.io/packagist/dt/nubs/which.svg?style=flat)](https://packagist.org/packages/nubs/which)
[![License](http://img.shields.io/packagist/l/nubs/which.svg?style=flat)](https://packagist.org/packages/nubs/which)

[![Dependency Status](https://www.versioneye.com/user/projects/53a01f7b83add749a300001e/badge.svg?style=flat)](https://www.versioneye.com/user/projects/53a01f7b83add749a300001e)

## Requirements
This library requires PHP 5.4, or newer.

## Installation
This package uses [composer](https://getcomposer.org) so you can just add
`nubs\which` as a dependency to your `composer.json` file or execute the
following command:

```bash
composer require nubs/which
```


## Usage
The included `which` executable works much like the standard which utility.  It
takes an arbitrary number of parameters and outputs the path to each of them.

```bash
$ ./bin/which more vim foo
/bin/more
/usr/bin/vim
foo not found
```

The command is configured as a binary with composer, so it is accessible in
`vendor/bin/which` when you install the package.  For a global install, this
means that you can find it in `$COMPOSER_HOME/vendor/bin/which`.  This command
does require the symfony/console package to be installed and accessible via the
autoloader.
