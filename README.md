## Iniciar proyecto para desarrollo local

1. Copiar .env.example a .env

        cp .env.example .env

2. Ejecutar el siguiente comando

        docker run --rm \
            -u "$(id -u):$(id -g)" \
            -v "$(pwd)":/var/www/html \
            -w /var/www/html \
            laravelsail/php82-composer:latest \
            composer install --ignore-platform-reqs

3. Alias para sail

        echo "alias sail='./vendor/bin/sail'" >> ~/.bashrc
        source ~/.bashrc

4. Iniciar el servidor local

        sail up

    Ejecutar en segundo plano

        sail up -d

        sail down

5. Generar key de Laravel

        sail artisan key:generate

6. Ejecutar migraciones de la base de datos

        sail artisan migrate

7. Instalar librerías de front

        sail npm i

8. Ejecutar build de front

        sail npm run build

    Live server

        sail npm run dev

9. Actualilzar cambios

        git pull
        sail composer insall # si hay paquetes php nuevos (cambios en composer.json)
        sail artisan migrate # si hay migraciones nuevas (nuevos archivos en /database/migrations)
        sail npm i           # si hay paquetes js nuevos (cambios en package.json)

10. Pruebas

    Abrir en un navegador

        http://localhost

    Panel de adminstración (backoffice)

        http://localhost/admin

    Crear usuario administrador

        sail artisan make:filament-user

    Ejecutar tests

        sail test
