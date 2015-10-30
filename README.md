# Which CLI
A PHP symfony/console command similar to the standard which command.

[![Build Status](http://img.shields.io/travis/nubs/which-cli.svg?style=flat)](https://travis-ci.org/nubs/which-cli)
[![Scrutinizer Code Quality](http://img.shields.io/scrutinizer/g/nubs/which-cli.svg?style=flat)](https://scrutinizer-ci.com/g/nubs/which-cli/)
[![Code Coverage](http://img.shields.io/coveralls/nubs/which-cli.svg?style=flat)](https://coveralls.io/r/nubs/which-cli)

[![Latest Stable Version](http://img.shields.io/packagist/v/nubs/which-cli.svg?style=flat)](https://packagist.org/packages/nubs/which-cli)
[![Total Downloads](http://img.shields.io/packagist/dt/nubs/which-cli.svg?style=flat)](https://packagist.org/packages/nubs/which-cli)
[![License](http://img.shields.io/packagist/l/nubs/which-cli.svg?style=flat)](https://packagist.org/packages/nubs/which-cli)

[![Dependency Status](https://www.versioneye.com/user/projects/53bdd76ce1d1583e8200028a/badge.svg?style=flat)](https://www.versioneye.com/user/projects/53bdd76ce1d1583e8200028a)

## Requirements
This script requires PHP 5.5, or newer.

## Installation
This package uses [composer](https://getcomposer.org) so you can install it
using composer.  Composer can install the command globally using:
```bash
composer global require nubs/which-cli
```

This will install it to your `$COMPOSER_HOME` directory (typically
`$HOME/.composer`).  The `which` binary will be symlinked to
`$COMPOSER_HOME/vendor/bin/which` (e.g., `$HOME/.composer/vendor/bin/which`).

## Usage
The included `which` executable works much like the standard which utility.  It
takes an arbitrary number of parameters and outputs the path to each of them.

```bash
$ which more vim foo
/bin/more
/usr/bin/vim
foo not found
```

For windows users, composer will create a `which.bat` script in
its bin directory that can be executed in much the same way as on a POSIX
system.  Alternatively, a `which.bat` script is included.  You may need to add
the `bin` directory from this repository to your `PATH` environment variable to
be able to access the command globally.

## License
which-cli is licensed under the MIT license.  See [LICENSE](LICENSE) for the
full license text.
