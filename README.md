# Ansible EUNERD

These are our infrastructure tasks and roles for provision our Rails apps using __nginx + unicorn__.

# TODO

  * [ ] https://github.com/dcarley/rbenv-sudo
  * [ ] export RAILS_ENV


## How to use

  * Fork this repository
  * ```mv group_vars_example group_vars```
  * Edit variables on ```group_vars/``` to fit your needs
  * Run site.yml, like ```ANSIBLE_NOCOWS=1 ansible-playbook -i staging site.yml```

### Roles

  - [geerlingguy.security](geerlingguy.security), tag: security
  - [nickjj.fail2ban](nickjj.fail2ban), tag: true, tags: fail2ban
  - [DavidWittman.redis](DavidWittman.redis), tag: redis
  - [nickhammond.logrotate](nickhammond.logrotate), tag: logrotate
  - [geerlingguy.java](geerlingguy.java), tag: java
  - [geerlingguy.elasticsearch](geerlingguy.elasticsearch), tag: elasticsearch
  - [franklinkim.openssl](franklinkim.openssl), tag: openssl
  - [jdauphant.nginx](jdauphant.nginx), tag: nginx
  - [franklinkim.nodejs](franklinkim.nodejs), tag: nodejs
  - [franklinkim.timezone](franklinkim.timezone), tag: timezone
  - [franklinkim.users](franklinkim.users), tag: users
  - [franklinkim.users-oh-my-zsh](franklinkim.users-oh-my-zsh), tag-zsh, tags: ohmyzsh
  - [franklinkim.ufw](franklinkim.ufw), tag: ufw
  - [zzet.rbenv](zzet.rbenv), tag: rbenv


### APT packages
  - build-essential
  - git-core
  - libxml2-dev
  - python-psycopg2
  - libpq-dev
  - imagemagick
  - zlib1g-dev
  - libssl-dev
  - libyaml-dev
  - libxml2-dev
  - bison
  - libreadline6
  - libreadline6-dev
