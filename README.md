# ansible-freebsd-read-only

Configuration a BSD system as a stateless system to save disk usage.

## Requirements

N.A.

## Role Variables


## Dependencies

N.A.

## Example Playbook

``` yaml
- hosts: servers
  roles:
  - role: ansible-bsd-read-only
```

## Testing

This role provides a `Vagrantfile` and a `Makefile`.

``` bash
# Makefile-provided commands
$ make help
help                This help message
lint                Test YAML syntax
vagrant-destroy     Destroy vagrant boxes
vagrant-variables   Test vagrant env variables
vagrant-vbox        Test the playbook using vagrant and virtualbox
# Mandatory variables
$ export VAGRANT_BOX_NAME="my-box"
# Optionnal variables
$ export VAGRANT_BOX_URL="http://repo/my-box.box"
$ export VAGRANT_VM_CPUS=5
$ export VAGRANT_VM_MEMORY=5120
# Vagrant using Virtualbox
$ make vagrant-vbox
$ make vagrant-destroy
```

## License

GPL-3+

## Author Information

Mathieu GRZYBEK
