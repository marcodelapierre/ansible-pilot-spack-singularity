# ansible-pilot-spack-singularity
A pilot Ansible playbook to install Spack, Singularity and SHPC (Singularity-HPC)

Note this playbook assumes Ubuntu/Debian based systems, and as such uses `apt` for package management.

To run the playbook:
```
ansible-playbook site.yaml
```

To run the playbook with sudo privileges required for some tasks:
```
ansible-playbook --ask-become-pass test.yaml
```

To generate a template configuration:
```
ansible-config init --disabled -t all >ansible_template.cfg
```
