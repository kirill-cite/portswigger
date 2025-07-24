# Lab 05 - Web shell upload via onfuscated file extension

## End goal: upload a basic PHP web shell and then use it to exfiltrate the contents of the file /home/carlos/secret

### Credentials - wiener:peter

1. Login and try to upload php shell/ You'll get error

2. Try different methods to obfuscate file extension

- exploit.php.jpg (double extension)
- exploit%2Ephp (URL- and double-URL encode)
- exploit.asp;.jpg and exploit.asp%00.jpg (semicolone and null byte)