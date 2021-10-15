# ansible-apps_dhcpd

## Description

[![Galaxy Role](https://img.shields.io/badge/galaxy-apps_dhcpd-purple?style=flat)](https://galaxy.ansible.com/lotusnoir/apps_dhcpd)
[![Version](https://img.shields.io/github/release/lotusnoir/ansible-apps_dhcpd.svg)](https://github.com/lotusnoir/ansible-apps_dhcpd/releases/latest)
![GitHub repo size](https://img.shields.io/github/repo-size/lotusnoir/ansible-apps_dhcpd?color=orange&style=flat)
[![downloads](https://img.shields.io/ansible/role/d/56087)](https://galaxy.ansible.com/lotusnoir/apps_dhcpd)
![Ansible Quality Score](https://img.shields.io/ansible/quality/56087)
[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen?style=flat)](https://opensource.org/licenses/Apache-2.0)


Deploy dhcpd using ansible.

## Requirements

none

## Role variables

| Name                      | Default Value | Description                        |
| ------------------------- | ------------- | -----------------------------------|
| `dhcpd_domain_name`       | "exemple.net" |  |

## Examples

	---
	- hosts: apps_dhcpd
	  become: yes
	  become_method: sudo
	  gather_facts: yes
	  roles:
	    - role: ansible-apps_dhcpd
	  environment: 
	    http_proxy: "{{ http_proxy }}"
	    https_proxy: "{{ https_proxy }}"
	    no_proxy: "{{ no_proxy }}


## License

This project is licensed under Apache License. See [LICENSE](/LICENSE) for more details.
