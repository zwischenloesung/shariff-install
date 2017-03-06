Shariff-Install
===============

The teams at c't and heise developed a free and open piece of software providing a fair way to use social media buttons - without leaking all personal data of all visitors (see https://github.com/heiseonline/shariff).

This role install the shariff-php backend onto your webserver.

STATUS: alpha
-------------

TODO
----

Well, we have only just begun.

Promise
-------

Sure, this role may change in the future, but we will only expand features to not break backwards compatibility.

If radical changes should become necessary, a new role will be created, probably with an 'ng' or version suffix...

Installation
------------

 # ansible-galaxy install zwischenloesung.shariff-install

Requirements
------------

* Ansible >2.2
* On target host
 * Generic UNIX with FHS
 * PHP (default config needs PHP 5.6/7.0/7.1, just change to older version if needed, shariff 3.0.1 supports PHP 5.4 for example)

Role Variables
--------------

* app\_\_shariff

Dependencies
------------

* Galaxy-Role: zwischenloesung.yapkg
 * Will install the php5 provider on debian (default \[ 'php5-fpm' \] use app\_\_php\_\_yapkg to overwrite)

Example Playbook
----------------

    - hosts: servers
      roles:
         - zwischenloesung.shariff-install

License
-------

GPLv3

Author Information
------------------

* Michael Lustenberger at [inofix.ch](http://www.inofix.ch)

