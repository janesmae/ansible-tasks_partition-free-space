# ansible-tasks_partition-free-space

Ansible partial tasklist to partition free space

## Sample playbook

```yaml
---

- name: Partition free disk
  hosts: hostname
  gather_facts: yes
  become: yes

  tasks:
    - { include_tasks: disk_partition_free_space.yml, vars: { device: /dev/sda, unit: MiB, vg: os } }
```

## License

MIT

## Authors

* Jaan Janesmae <jaan@janesmae.com>
