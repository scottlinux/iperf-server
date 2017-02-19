Role Name
=========

Instant iperf server!

This playbook provides a temporary iperf3 server to use for network testing.

Currently, Fedora Linux is the tested iperf server for this playbook.

Requirements
------------

Fedora 25+ for iperf server

Ansible 2.2.0+ to run playbook

Role Variables
--------------

n/a

Dependencies
------------

Fedora packages: 

    python2-dnf ansible python-firewall git

Example Playbook
----------------

Run playbook to provision an iperf server!

From inside provisioned VM or added to automation:

    ansible-pull -i 'localhost,' -c local -d /tmp/iperf-server -U https://github.com/scottlinux/iperf-server

From one's workstation to provision a remote VM:

    git clone https://github.com/scottlinux/iperf-server
    ansible-playbook -i "ip.address.of.iperf.server.vm," iperf-server/local.yml
    
    
License
-------

MIT

Author Information
------------------

@scottlinux
