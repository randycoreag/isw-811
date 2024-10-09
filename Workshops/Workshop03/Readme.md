# Workshop 03

![Virtualizacion](./images/header.png)

## Realizar las Respectivas Configuraciones

- `sudo nano /etc/hosts:` este comando lo utilizo para editar el archivo del host de la maquina
- `192.168.56.199  lfts.isw811.xyz :` esta linea la agregamos en el archivo hosts de la maquina anfitriona para similiar el dominio que queremos utilizar, esto lo podemos probar con realizar un ping a dicho dominio para probar su funcionamiento.
- Realizamos una prueba ingresando desde el navegador en una venta en incognito a cualquiera de los dos dominios que tenemos configuradas
- `cd /vagrant/:` para irnos a la raiz de vagrant, aca podemos ver que todo lo que pongamos en la maquina anfitriona la podemos observar tambien desde el servidor
- `touch lfts.isw811.xyz.conf:` para crear el archivo de configuracion de las paginas que vamos a tener almacenadas
- `sudo cp lfts.isw811.xyz.conf /etc/apache2/sites-available/ :` copiamos el archivo para poder habilitar el sitio
- `sudo a2ensite lfts.isw811.xyz :` este comando es para habilitar el sitio
- `sudo apache2ctl -t:` para verificar que todo este ok
- `systemctl reload apache2:` lo utilizamos para reiniciar el servicio de apache

## Laravael 

- `php -v :` comando para verificar la version de PHP

- `php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"`
- `php -r "if (hash_file('sha384', 'composer-setup.php') === - 'dac665fdc30fdd8ec78b38b9800061b4150413ff2e3b6f88543c636f7cd84f6db9189d43a81e5503cda447da73c7e5b6') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"`
- `php composer-setup.php`
- `php -r "unlink('composer-setup.php');"`:comandos para descargar composer
- `./composer.phar :` para ejecutar el composer en el directorio actual
- `echo $PATH :` contenido de la variable de entorno PATH
- `sudo mkdir -p /opt/composer: ` crear carpeta
- `sudo mv composer.phar /opt/composer :` mover el binario a la carpeta anteriormente creada
- `sudo ln -s /opt/composer/composer.phar /usr/local/bin/composer :` crear lanzador
- `composer create-project laravel/laravel:8.6.12 lfts.isw811.xyz :` comando para crear el projecto de laravel 

## Prueba de la Finalizacion de la Publicacion de la Pagina Web

![Virtualizacion](./images/lospatitos.com.png)