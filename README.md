get-external-ip-via-opendns
=========

Add fact about machine: external (white) IPv4 address via opendns server.

Address exported as 'external_ip' 

Requirements
------------

Machine should have working external network and should be able to send DNS requests (UDP/53). Opendns service should works.
Machine should have dig utility installed.

Role Variables
--------------

dns_selfip_resolver (default to resolver1.opendns.com)

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: get-external-ip-via-opendns }

License
-------

BSD

Author Information
------------------

(c) George Shuklin, 2015
