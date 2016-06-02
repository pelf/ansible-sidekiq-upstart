# Ansible role to install Sidekiq

This Ansible role installs/updates Sidekiq.  It also copies a working Upstart script.

## Installation

``` bash
$ ansible-galaxy install pelf.sidekiq-upstart,v1.0.0
```

## Variables

``` yaml
app_name: test
app_path: /home/ubuntu/test
deploy_user: deploy
server_env: qa
app:
  process_name: "{{ app_name }}"
```

## Usage

Once this role is installed on your system, include it in the roles list of your playbook.

``` yaml
- hosts: localhost
  roles:
    - pelf.sidekiq-upstart
```

## Dependencies

None

## License

MIT
