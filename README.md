Wallabag Bastille Template
--------------------------

Template for [Wallabag](https://wallabag.org) application configured with Nginx,
PostgreSQL and PHP-FPM. For PostgreSQL, you need to activate `sysvshm` with:

```
bastille config <target> set sysvshm new && bastille restart <target>
```

before applying this template.

## Template variables

List of variables of this template:

 * `WALLABAG_VERSION`: version of wallabag to install
 * `DBNAME`, `DBUSER`, `DBPASS`: database parameters
 * `SECRET`: value of Wallabag secret parameter
 * `FQDN`: domain name for Wallabag
 * `LOCALE`: locale for wallabag parameter
