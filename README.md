# aes-php-js-encryption
AES Encryption &amp; Decryption using PHP and JS

### How to use

- Include the library file in the page
- Call the function with a passkey in PHP and JavaScript

# Exapmle


#### USING PHP

Include the libeary before `include('encryption.php');`

    <?php
		$data = "Welcome";
		$passkey = "MySecretKey";
		$encrypted_value = PHPAESKey::enc($data, $passkey);
    ?>
    
Resut (Every time you call the mentod it will give diferent encrypted string):

    U2FsdGVkX19lv+Yd4vzJl1K9VqDuce0MPjVbCU1YmN4=
    // output result
####Using Javascript　

```javascript
<script src="encryption.js"></script>
<script>
	var paskey = "MySecretKey";
	var theValue = JSAESKey .dec('<?=encrypted_value?>', paskey);
	console.log(theValue);
</script>
```
Resut  in console
```javascript
Welcome
```


