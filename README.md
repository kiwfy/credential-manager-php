# PHP Credential Manager

[![Latest Version](https://img.shields.io/packagist/v/kiwfy/credential-manager-php?style=flat-square&label=Latest%20Version)](https://github.com/kiwfy/credential-manager-php/releases)
[![CI Build](https://img.shields.io/circleci/build/github/kiwfy/credential-manager-php/master?label=CI%20Build&token=34d8b3820b7229d742897f0a6982ced5bf6a99c8)](https://github.com/kiwfy/credential-manager-php)
[![codecov](https://codecov.io/gh/kiwfy/credential-manager-php/branch/master/graph/badge.svg?token=O47QIGFACQ&label=Codecov)](https://codecov.io/gh/kiwfy/credential-manager-php)
[![Total Downloads](https://img.shields.io/packagist/dt/kiwfy/credential-manager-php.svg?style=flat-square&label=Total%20Downloads)](https://packagist.org/packages/kiwfy/credential-manager-php)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square&label=PRs%20Welcome)](http://makeapullrequest.com)

PHP library for search credential in redis with Predis.

### Installation

Requires [PHP](https://php.net) 7.1

The recommended way to install is through [Composer](https://getcomposer.org/).

```sh
composer require kiwfy/credential-manager-php
```

### Sample

it's a good idea to look in the sample folder to understand how it works.

First you need to building a correct environment to install dependences

```sh
docker build -t kiwfy/credential-manager-php -f contrib/Dockerfile .
```

Access the container
```sh
docker run -v ${PWD}/:/var/www/html -it kiwfy/credential-manager-php bash
```

Verify if all dependencies is installed (if need anyelse)
```sh
composer install --no-dev --prefer-dist
```

and run
```sh
php sample/CredentialSample.php
php sample/CredentialRedisConfigSample.php
```

### Development

Want to contribute? Great!

The project using a simple code.
Make a change in your file and be careful with your updates!
**Any new code will only be accepted with all viladations.**

To ensure that the entire project is fine:

First you need to building a correct environment to install/update all dependences
```sh
docker build -t kiwfy/credential-manager-php -f contrib/Dockerfile .
```

Access the container
```sh
docker run -v ${PWD}/:/var/www/html -it kiwfy/credential-manager-php bash
```

Install all dependences
```sh
composer install --dev --prefer-dist
```

Run all validations
```sh
composer check
```

**Kiwfy - Open your code, open your mind!**
