1. con la siguiente linea de comandos crearemos el modelo y controlador
en este caso lo llamaremos de nombre Product

 	php artisan make:model Product -mc

2. para cargar datos semilla

	php artisan make:seeder ProductsTableSeeder


3. procedemos a refrescar y crear la migracion en la base de datos

	php artisan migrate:refresh --seed

4. definimos las rutas del crud

	 php artisan route:list

5. procederemos a usar las vistas de crear y editar para eso usaremos el paquete de laravel collective

	composer require "laravelcollective/html":"^5.4.0"


	Next, add your new provider to the providers array of config/app.php:

  	'providers' => [
    		// ...
    		Collective\Html\HtmlServiceProvider::class,
    		// ...
  	],

	Finally, add two class aliases to the aliases array of config/app.php:

  	'aliases' => [
    		// ...
      		'Form' => Collective\Html\FormFacade::class,
      		'Html' => Collective\Html\HtmlFacade::class,
    		// ...
  		],


6. validaciones en los campos del formulario

	php artisan make:request ProductRequest

7. traducir a diferentes idiomas - configurar idioma español

	Descargar la carpeta "es" copiarla en resource->lang

	https://github.com/italomoralesf/Laravel-lang




