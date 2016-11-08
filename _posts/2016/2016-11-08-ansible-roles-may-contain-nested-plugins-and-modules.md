---
layout: "post"
title: "Ansible roles may contain nested plugins and modules"
date: "2016-11-08 17:05"
---

Sooner or later, you're going to ask yourself **Is it possible to import remote *Ansible modules* to use them on my playbook**

Yes, you can.
http://stackoverflow.com/a/36160664

If desired, you can for instance call this (taken from a remote git repository) Ansible action_plugin that allows you to reconnect ssh connections:

https://galaxy.ansible.com/udondan/ssh-reconnect/


It's up to you if you use `ansible-galaxy` to install the remote action_plugin, [as described on the docs](http://docs.ansible.com/ansible/galaxy.html#version):



```ansible-galaxy install git+https://github.com/geerlingguy/ansible-role-apache.git,0b7cd353c0250e87a26e0499e59e7fd265cc2f25```


Or if you prefer to [specify a list of role dependencies][3a5c7b4b] in the `meta/main.yml` file

  [3a5c7b4b]: http://docs.ansible.com/ansible/galaxy.html#dependencies "Specify a list of Ansible role dependencies"

```dependencies:
  - src: geerlingguy.ansible
  - src: git+https://github.com/geerlingguy/ansible-role-composer.git
    version: 775396299f2da1f519f0d8885022ca2d6ee80ee8
    name: composer
```

Give it a try and may the force be with you!
