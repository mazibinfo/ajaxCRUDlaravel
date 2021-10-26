## create project
### `composer create-project --prefer-dist laravel/laravel ajaxcrud`

## Install Yajra Datatable
### `composer require yajra/laravel-datatables-oracle`

## config/app.php

'providers' => [\
	Yajra\DataTables\DataTablesServiceProvider::class,\
]\
'aliases' => [\
	'DataTables' => Yajra\DataTables\Facades\DataTables::class,\
]

## Create Migration Table
### `php artisan make:migration create_products_table --create=products`
### `php artisan migrate`

## Create Route
### `Route::resource('ajaxproducts','ProductAjaxController');`

## Add Controller and Model
### `php artisan make:model Product`
### `php artisan make:controller ProductAjaxController`
