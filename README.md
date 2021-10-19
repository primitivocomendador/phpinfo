# phpinfo

```
git clone https://github.com/primitivocomendador/phpinfo
cd phpinfo
git checkout main
```
```
php -f src/index.php -S 0.0.0.0:8080
```
```
curl localhost:8080/src/index.php
```
Instruciones para construir imagen Docker
```
git checkout santander
docker build --file Dockerfile --tag primitivocomendador/phpinfo:santander .
```
Instruciones para arrancar el Docker:
´´´´
docker run -d --entrypoint /usr/bin/php --name phpinfo -p 8080:8080 -v &{PWD}/src/index.php:/src/index.php:ro primitivocomendador/phpinfo:santander -f src/index.php -S 0.0.0.0:8080
´´´´
