Ansible Role: upower_charge_thresholds
=========

Ansible role to set batteries charge thresholds on Linux using upower

Requirements
------------

This role requires UPower >= 1.90 to be installed on target machines

Role Variables
--------------

```yaml
upower_charge_thresholds_start_threshold: 40
```
The start threshold value (percentage): batteries will start charge level drops under this threshold.

```yaml
upower_charge_thresholds_stop_threshold: 50
```
The "stop" threshold value (percentage): batteries will stop charging when this level is reached.

Dependencies
------------

None

Example Playbook
----------------

    - hosts: all
      roles:
         - role: egdoc.upower_charge_thresholds

License
-------

GPLv2

Author Information
------------------
Written by Egidio Docile.
