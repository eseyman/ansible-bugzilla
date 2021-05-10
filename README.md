ansible-role-bugzilla
=========

This role will deploy an instance of Bugzilla.
It is based in the official documentation and daily experiences.
This role will be in continually improvement since now! Any help is welcome!

This role has been tested on the following operating systems:
- Fedora

I would like this role to support the following systems:
- CentOS and Red Hat
- Ubuntu
- Debian

Any other operating system support is welcome. If you want to work on this,
please submit a PR in the official repo (GitHub).

This role will:
- Install the Apache HTTPD web server
- Git-clone a copy of the Bugzilla software
- Run checksetup.pl
- Configure Bugzila to use the configured database

Requirements
------------

- python3
- Internet Access to the Bugzila repo on GitHub

Role Variables
--------------

You can customize your environment in a very simple and centralized way editing some variables in:
- defaults/main.yml

In some rare cases, you may change some configuration to reflect your local environment in:
- vars/*.yml

Observe that the above variables could be set in your playbook too, which, IMO is much more elegant. ; )
Take a look in the Example Playbook section.

Dependencies
------------

None

Example Inventory
----------------

You can see a complete example inventory file inside the "files" folder.

Example Playbook
----------------

This playbook will prepare everything with the right variables. For this example, lets call
this playbook file as "ansible_bugzilla.yml" (an example file is in "files" folder).

License
-------

This Source Code Form is licensed under the same terms as Bugzilla itself.

Author Information
------------------

- Emmanuel Seyman - emmanuel+github@seyman.fr
