1. composer create-project laravel/laravel .

2. .env

3.  Multiple Authentication Guards

3.1 composer create-project --prefer-dist laravel/laravel multi-guard-auth

3.2 composer require laravel/ui

3.3 php artisan ui bootstrap --auth

3.4 npm install

3.5 php artisan make:model Admin -m

3.6 Authentication: config/auth.php

3.7 LoginController 

3.8 RegisterController

3.9 login.blade.php

3.10 register.blade.php

3.11 touch resources/views/admin.blade.php

3.12 home.blade.php

3.13 web.php (admin route)

3.14 RedirectIfAuthenticated.php Middleware

3.15 authentication exception handler: app/Exceptions/Handler.php

3.16 npm run dev

#The Vite plugin requires Node 16.15.1 or greater.
sudo npm cache clean -f
sudo npm install -g n
sudo n stable

sudo n latest

#tinker

php artisan tinker

$admin = new App\Models\Admin;
$admin->name = "john joe";
$admin->email = "admin@admin.com";
$admin->email_verified_at = now();
$admin->password = Hash::make("12345678");
$admin->save();