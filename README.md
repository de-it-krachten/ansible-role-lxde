[![CI](https://github.com/de-it-krachten/ansible-role-lxde/workflows/CI/badge.svg?event=push)](https://github.com/de-it-krachten/ansible-role-lxde/actions?query=workflow%3ACI)


# ansible-role-lxde

<basic role description>



## Dependencies

#### Roles
None

#### Collections
None

## Platforms

Supported platforms

- Red Hat Enterprise Linux 8<sup>1</sup>
- Red Hat Enterprise Linux 9<sup>1</sup>
- Red Hat Enterprise Linux 10<sup>1</sup>
- RockyLinux 8
- RockyLinux 9
- RockyLinux 10
- OracleLinux 8
- OracleLinux 9
- OracleLinux 10
- AlmaLinux 8
- AlmaLinux 9
- AlmaLinux 10
- Debian 11 (Bullseye)
- Debian 12 (Bookworm)
- Debian 13 (Trixie)
- Ubuntu 22.04 LTS
- Ubuntu 24.04 LTS
- Ubuntu 26.04 LTS
- Fedora 43
- Fedora 44<sup>1</sup>

Note:
<sup>1</sup> : no automated testing is performed on these platforms


## Role Variables
### defaults/main.yml
<pre><code>
lxde_user: vagrant
lxde_group: vagrant
lxde_monitor: Virtual1
lxde_monitor_mode: '1920x1080'
lxde_monitor_rate: '60.00'
</pre></code>




## Example Playbook
### molecule/default/converge.yml
<pre><code>
- name: sample playbook for role 'lxde'
  hosts: all
  become: 'yes'
  tasks:
    - name: Include role 'lxde'
      ansible.builtin.include_role:
        name: lxde
</pre></code>
