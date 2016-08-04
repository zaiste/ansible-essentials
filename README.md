ansible-essentials
=========

An Ansible role that installs essential elements (libraries and packages) on Ubuntu Xenial.

Requirements
------------

None.

Role Variables
--------------

- `essential_libraries` defaults to:
  ```
  - software-properties-common
  - python-software-properties
  - build-essential
  - libreadline-dev
  - libssl-dev
  - libsqlite3-dev
  - sqlite3
  - libyaml-dev
  - libxml2-dev
  - libxslt1-dev
  - zlib1g-dev
  - apt-transport-https
  - ca-certificates
  ```

- `essential_packages` defaults to
  ```
  - curl
  - fail2ban
  - mosh
  - vim
  - git
  - git-core
  - imagemagick
  - ufw
  ```

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: zaiste.essentials }

License
-------

MIT / BSD

Author Information
------------------

[Zaiste](http://zaiste.net) 2014 - 2016
