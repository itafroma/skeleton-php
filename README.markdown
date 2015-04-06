# Skeleton project (PHP)

This is a placeholder/skeleton project to load the essential configuration and packages [I][1] use for development of PHP projects.

## Conventions

### Dependencies

- [Composer][2] for dependency management
- [PSR-4][3] for autoloading
- [PHPUnit][4] for unit-testing
- [Scrutinizer][5] for code analysis and reporting, configured to match [PSR-1][6] and [PSR-2][7] (among other things: see [.scrutinizer.yml](./.scrutinizer.yml))
- [Travis CI][8] for continuous integration

### Directory structure:

- [bin](./bin): Executable artifacts
- [build](./build): Automatically generated artifacts from your build/CI process. For example, PHPUnit test results will be placed here.
- [config](./config): Configuration files that are not required to be in the project root
- [src](./src): PSR-4-compliant code
- [tests](./tests): PSR-4-compliant PHPUnit tests
- [vendor](./vendor): Dependency artifacts from Composer

## Usage

First, load this package as a project via Composer:

```sh
# Replace [PROJECT] with the desired name of your project directory
composer create-project itafroma/skeleton [PROJECT]
```

Remove the existing VCS history when asked: this information is specific to this repository, not your new project.

Next, modify the existing files to be specific to your new project:

* [composer.json](./composer.json)
* [LICENSE](./LICENSE)
* [README.markdown](./README.markdown)

Finally, update your project's `composer.lock`:

```sh
composer update
```

Now you're ready to start development and push your new project to your favorite VCS.

## Copyright and license

Where applicable, this project is released into the public domain. It is otherwise made available via the MIT license. A copy of the license can be found in the [LICENSE](./LICENSE) file.

[1]: https://marktrapp.com "My website"
[2]: https://getcomposer.org "Composer website"
[3]: http://www.php-fig.org/psr/psr-4/ "PSR-4 specification"
[4]: https://phpunit.de "PHPUnit website"
[5]: https://scrutinizer-ci.com "Scutinizer website"
[6]: http://www.php-fig.org/psr/psr-1/ "PSR-1 specification"
[7]: http://www.php-fig.org/psr/psr-2/ "PSR-2 specification"
[8]: https://travis-ci.org "Travis CI website"
