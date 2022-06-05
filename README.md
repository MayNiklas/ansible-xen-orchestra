install xen-orchestra via ansible
=========

This role installs xen-orchestra on a Debian or Ubuntu server.
The software is getting build from source. To understand the implications, please read: [xen-orchestra from source](https://xen-orchestra.com/docs/installation.html#from-the-sources)

Requirements
------------

Tested on:
- Debian 10
- Debian 11
- Ubuntu 20.04
- Ubuntu 22.04

Role Variables
--------------

| variable        | description                                    | default                                  |
|-----------------|------------------------------------------------|------------------------------------------|
| nodejs_version: | nodejs version to install                      | 16.x                                     |
| xo_path:        | path xen-orchestra gets cloned to / build from | /usr/local/xen-orchestra                 |
| xo_user:        | user under which xen-orchestra runs            | xen-orchestra                            |
| xo_group:       | group under which xen-orchestra runs           | xen-orchestra                            |
| xo_branch:      | branch to build from                           | master                                   |
| xo_server:      | git repository                                 | https://github.com/vatesfr/xen-orchestra |

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
