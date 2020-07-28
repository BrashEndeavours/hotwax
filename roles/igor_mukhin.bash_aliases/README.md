    # ansible-role-bash_aliases

Ansible role for setting aliases in ~/.bash_aliases for Debian/Ubuntu.

## Prerequisites

First of all you should install [Ansible](http://www.ansible.com/home) on your machine, official [docs](http://docs.ansible.com/intro_installation.html) should help you with that.

# Installation
```bash
ansible-galaxy install igor_mukhin.bash_aliases
```

## Example playbook

Lets make aliases for most used symfony2 console commands

```yml
# playbook.yml

vars:
	# See all available variables at defaults/main.yml
	bash_aliases:
	  - { alias: 'sf', command: 'php app/console' }

	  - { alias: 'sfcc', command: 'sf cache:clear' }
	  - { alias: 'sfccnw', command: 'sfcc --no-warmup' }

	  - { alias: 'sfl', command: 'sf list' }
	  - { alias: 'sflg', command: 'sf list | grep' }

    # You also can add extra lines in any format to .bash_aliases
    bash_aliases_extra:
      - "git config --global alias.unstage 'reset HEAD --'"

roles:
  - { role: igor_mukhin.bash_aliases, sudo: false }

```
