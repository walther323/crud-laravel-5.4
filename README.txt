1. con la siguiente linea de comandos crearemos el modelo y controlador
en este caso lo llamaremos de nombre Product

 	php artisan make:model Product -mc

2. para cargar datos semilla

	php artisan make:seeder ProductsTableSeeder


3. procedemos a refrescar y crear la migracion en la base de datos

	php artisan migrate:refresh --seed

4. definimos las rutas del crud

	 php artisan route:list





