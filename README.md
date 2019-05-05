# laravel-npm-run
[![Latest Version on Packagist](https://img.shields.io/packagist/v/repat/laravel-npm-run.svg?style=flat-square)](https://packagist.org/packages/repat/laravel-npm-run)
[![Total Downloads](https://img.shields.io/packagist/dt/repat/laravel-npm-run.svg?style=flat-square)](https://packagist.org/packages/repat/laravel-npm-run)

**laravel-npm-run** is a package that runs e.g. `npm run dev` or `npm run production` as a Laravel Queued Job, using [symfony/process](https://symfony.com/doc/current/components/process.html). For documentation see:

* https://laravel.com/docs/5.8/mix
* https://laravel.com/docs/5.8/queues

## Installation
`$ composer require repat/laravel-npm-run`

## Documentation
There are multiple ways to create and dispatch a Job, please see [Laravel Documentation on Queues](https://laravel.com/docs/5.8/queues).

```php
// Create Job
$job = new \Repat\Jobs\NpmRun(config('app.env'));
$job = new \Repat\Jobs\NpmRun(); // env = dev

// Dispatch Job
dispatch($job);
$job->dispatch();
$this->dispatch($job); // e.g. in Controller
```

## License
* MIT, see [LICENSE](https://github.com/repat/laravel-npm-run/blob/master/LICENSE)

## Version
* Version 0.1

## Contact
#### repat
* Homepage: https://repat.de
* e-mail: repat@repat.de
* Twitter: [@repat123](https://twitter.com/repat123 "repat123 on twitter")

[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=repat&url=https://github.com/repat/laravel-npm-run&title=laravel-npm-run&language=&tags=github&category=software)
