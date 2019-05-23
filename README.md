# spring-cloud-config-store

spring-cloud-config-store is use for remotely access to the configuration files for updating purposes by
regarding to relevent profile and application name.

```bash
eg: profile= prod, dev, qa or the default 
    application name= item, stock or stack 
```
## Prerequisite

Please refer below link and download the particular Java Cryptography Extension (JCE) jar files
( https://www.oracle.com/technetwork/java/javase/downloads/jce-all-download-5170447.html.) and
put those jar files into the JRE security folder, and restart the application.


## Change the sensitive details of the configration files in repository

1. copy the password in to the post request body using the config server encrypt endpoint and generate the Hash value.
  ```bash
  eg: config server encrypt endpoint= http://localhost:8091/encrypt 
      Body= 1qaz2wsx@
      Output= 957b3c8c1c83734b3e1dfb5ad6297248a852d1566bfcde488c3fb49e0a67cd09
  ```
2. Copy the hash value with the prefix " {cipher} " and replace with the previous plain password and commit in to repository 
    as <b>.properties</b> file
  ```bash
      
  ```

## Usage

```python
import foobar

foobar.pluralize('word') # returns 'words'
foobar.pluralize('goose') # returns 'geese'
foobar.singularize('phenomena') # returns 'phenomenon'
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[No]
