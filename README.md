## Usage


```bash	```bash
php password-generator.php --length=<length>	php password-generator.php --length=<length> --chars=<character-mapping-key>
```	```


### Password Length (`--length`)	### Password Length (`--length`)
@@ -14,13 +14,26 @@ To pass the desired password length, use the `--length` option as shown in the e
A valid integer should be used. If an invalid integer is passed (or no length is passed at all),	A valid integer should be used. If an invalid integer is passed (or no length is passed at all),
the default of `12` will be used instead.	the default of `12` will be used instead.


### Character Mapping (`--chars`)

The character mapping keys are defined as follows:

- `numeric` - Numbers only
- `lowercase` - Lowercase letters only
- `uppercase` - Uppercase letters only
- `alpha` - Letters only
- `alphanumeric` - Numbers and letters only
- `special` - Special characters only

If no mapping is specified, the script will generate a password using all characters.

## Example	## Example
```bash	```bash
php password-generator.php --length=32	php password-generator.php --length=32 --chars=uppercase
```	```


Which would output something similar to:	Which would output something similar to:


```	```
?W@lnAcDgD^hR=vH^EtCms(/1qN_xF)l	FHNXIJNOCCBFLTJXWEWFQWMVQCOIQMOK
```	```
