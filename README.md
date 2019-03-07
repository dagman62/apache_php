Role Name
=========

Apache PHP install from source

Role Variables
--------------

apache_version: httpd-2.4.38
apr_version: apr-1.6.5
apru_version: apr-util-1.6.1
php_version: php-7.2.15
php_tarball_url: "http://php.net/get/{{ php_version }}.tar.gz/from/this/mirror"
php_install_dir: "/tmp/{{ php_version }}"
apache_tarball_url: "http://www-us.apache.org/dist/httpd/{{ apache_version }}.tar.gz"
apache_install_dir: "/tmp/{{ apache_version }}"
apr_tarball_url: "http://www-us.apache.org/dist/apr/{{ apr_version }}.tar.gz"
apr_install_dir: "/tmp/{{ apr_version }}"
apru_tarball_url: "http://www-us.apache.org/dist/apr/{{ apru_version }}.tar.gz"
apru_install_dir: "/tmp/{{ apru_version }}"
apache_user: "www-data"
apache_group: "www-data"
apache_home: "/opt/apache"
apache_email: "admin@example.com"

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: apache_php }

License
-------

BSD

Author Information
------------------

Gaetano Giacalone
https://dagman62.com