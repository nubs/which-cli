# Which
A PHP library for locating commands in a PATH.

[![Build Status](https://travis-ci.org/nubs/which.png)](https://travis-ci.org/nubs/which)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/nubs/which/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/nubs/which/?branch=master)
[![Code Coverage](https://scrutinizer-ci.com/g/nubs/which/badges/coverage.png?b=master)](https://scrutinizer-ci.com/g/nubs/which/?branch=master)

[![Latest Stable Version](https://poser.pugx.org/nubs/which/v/stable.png)](https://packagist.org/packages/nubs/which)
[![Total Downloads](https://poser.pugx.org/nubs/which/downloads.png)](https://packagist.org/packages/nubs/which)
[![Latest Unstable Version](https://poser.pugx.org/nubs/which/v/unstable.png)](https://packagist.org/packages/nubs/which)
[![License](https://poser.pugx.org/nubs/which/license.png)](https://packagist.org/packages/nubs/which)

[![Dependency Status](https://www.versioneye.com/user/projects/53a01f7b83add749a300001e/badge.svg?style=flat)](https://www.versioneye.com/user/projects/53a01f7b83add749a300001e)

## Requirements
This library requires PHP 5.3, or newer.

## Installation
This package uses [composer](https://getcomposer.org) so you can just add
`nubs\which` as a dependency to your `composer.json` file.

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
