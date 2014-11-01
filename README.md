Install with ```composer install```.

Import this database dump:
https://dl.dropboxusercontent.com/u/975953/magento_sample_data_for_1.9.0.0_with_media.sql.tar.bz2

Update url site to match ServerName with:

```SQL
UPDATE core_config_data SET value = 'http://magentodemo.dev/'
WHERE path LIKE 'web/secure/base_url';

UPDATE core_config_data SET value = 'http://magentodemo.dev/'
WHERE path LIKE 'web/unsecure/base_url';
```
