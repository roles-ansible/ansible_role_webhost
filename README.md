Web Host
========


Variables
---------


Example
-------

```
nginx_sites:
  - name: 'example.org'
    webroot:
      path: '/srv/www/example.org'
      user: 'webmaster'
      group: 'www-data'
      mode: 'u=rwx,g=rx,o=rx'

  - name: 'example.com'
    webroot: true
```


Note
----

Configuration data for this role should be included into the `nginx_sites` variable used inside the `nginx_new2` role.
