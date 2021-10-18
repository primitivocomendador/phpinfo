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
