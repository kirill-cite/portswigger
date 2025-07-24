# Lab 03: Web shell upload via path traversal

## Submit the simple PHP web shell and get /home/carlos/secret file

### Credentials - wiener:peter

1. Explre website and analyse file upload functionality

2. PHP file in user directory is under control

3. We need to move from our directoru ../filename.php

4. We need to encode '../' to bypass filtration - using URL-encode

