# ansible role debuild_rofi
Ansible cookbook to build and install a rofi .deb for Ubuntu/Debian.

# example
## playbook.yml
I install rofi on all hosts in the desktop group.
```yaml
- hosts: desktop
  roles:
    - derbunman.debuild_rofi
```

## requirements.yml
```yaml
- src: derbunman.debuild
- src: derbunman.debuild_rofi
```

## install dependencies
```sh
ansible-galaxy install -r requirements.yml
```

## update dependencies
```sh
ansible-galaxy install -r requirements.yml --force
```

## run playbook
```sh
ansible-playbook playbook.yml -v
```
