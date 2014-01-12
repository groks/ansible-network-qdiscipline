network-qdiscipline
========

An [ansible role](https://galaxy.ansibleworks.com/list#/roles/215) which sets
the queueing discipline on network interfaces to favour low latency over
ultimate bandwidth, hopefully benefiting interactive applications such as voice
calls, ssh etc. It enables the
[fq_codel](https://www.bufferbloat.net/projects/codel/wiki) algorithm.

This is a modification of
[M D Taht's public domain Debian script](https://github.com/dtaht/deBloat) to
work under NetworkManager on Fedora.

    ---
    - hosts: localhost

      roles:
        - groks.network-qdiscipline

Requirements
------------

An installation of [Fedora](https://fedoraproject.org/get-fedora) Linux.

Role Variables
--------------

None.

Dependencies
------------

None.

License
-------

BSD
