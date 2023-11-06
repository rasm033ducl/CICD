# Unit Test Examples

Example code for my talks and workshops on unit testing.

## Getting Started

Clone this repository, or download the ZIP file.

There is both PHP and JavaScript example code waiting for you at `src/php/` and `src/js/`, respectively.

## Writing Tests

The repository is set up for you to write PHP tests with [PHPUnit](https://github.com/sebastianbergmann/phpunit), and JavaScript tests with [Jest](https://github.com/facebook/jest).
If you would rather use something else instead, feel free to adapt `composer.json` and `package.json`, respectively.

### PHP Tests

In order to run the PHP tests, you have to install the required PHP packages first.

Install with [Composer](https://getcomposer.org/):

```shell
$ composer install
```

By default, this will install PHPUnit as well as [Mockery](https://github.com/mockery/mockery), [Patchwork](https://github.com/antecedent/patchwork/) and [Brain Monkey](https://github.com/Brain-WP/BrainMonkey).

Then, execute PHPUnit, which will use the configuration provided in `phpunit.xml.dist`:

```shell
$ ./vendor/bin/phpunit
```

### JavaScript Tests

In order to run the JavaScript tests, you have to install the required JavaScript packages first.

Install with [Yarn](https://github.com/yarnpkg/yarn):

```shell
$ yarn
```

By default, this will install Jest (inlcuding [`jest-each`](https://github.com/mattphillips/jest-each)), [`react-test-renderer`](https://github.com/facebook/react/tree/master/packages/react-test-renderer) and [Enzyme](https://github.com/airbnb/enzyme) (including [`enzyme-adapter-react-16`](https://github.com/airbnb/enzyme/tree/master/packages/enzyme-adapter-react-16)), as well as the [`babel-preset-env`](https://github.com/babel/babel/tree/master/packages/babel-preset-env) and [`babel-preset-react`](https://github.com/babel/babel/tree/master/packages/babel-preset-react) packages.

Then, run the `test` script, defined in `package.json`:

```shell
$ yarn test
```

----

In case you want to use [npm](https://github.com/npm/npm) instead, do it like so:

```shell
$ npm i && npm run test
```

## License

Copyright (c) 2018 Thorsten Frommen

This code is licensed under the [MIT License](/LICENSE).
