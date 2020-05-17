# Laravel 7 and Svelte 3 SPA boilerplate using Inertia

A ready to develop [Laravel](https://laravel.com/) and [Svelte](https://svelte.dev/) SPA using [Inertia](https://inertiajs.com/)

## Installation

Clone the repo

```shell script
git clone https://github.com/djiwan/laravel-svelte.git
cd laravel-svelte
```

Install PHP dependencies:

```shell script
composer install
```

Install NPM dependencies:

```shell script
npm install
```

Build assets:

```shell script
npm run dev
```

Setup configuration:

```shell script
cp .env.example .env
```

Generate application key:

```shell script
php artisan key:generate
```

Run artisan server:

```shell script
php artisan serve
```

You're ready to go! Open browser and check the following address. http://localhost:8100

## Credits
- [laravel-mix-svelte](https://github.com/wewowweb/laravel-mix-svelte) by We Wow Web
