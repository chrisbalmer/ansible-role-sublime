Role Name
=========

Installs sublime-text and sublime-merge tools.

Requirements
------------

None

Role Variables
--------------

```
channel: stable
```

Whether to use the `stable` or `dev` repo channel.

```
sublime_text:
  state: latest
sublime_merge:
  state: latest
```

What products to install.

```
apt:
  gpg_key: https://download.sublimetext.com/sublimehq-pub.gpg
  stable: https://download.sublimetext.com/ apt/stable/
  dev: https://download.sublimetext.com/ apt/dev/

rpm:
  gpg_key: https://download.sublimetext.com/sublimehq-rpm-pub.gpg
  stable: https://download.sublimetext.com/rpm/stable/x86_64/sublime-text.repo
  dev: https://download.sublimetext.com/rpm/dev/x86_64/sublime-text.repo
```

Repo keys and locations for doing the installations.

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - { role: chrisbalmer.sublime }

License
-------

MIT

Author Information
------------------

Chris Balmer

https://github.com/chrisbalmer