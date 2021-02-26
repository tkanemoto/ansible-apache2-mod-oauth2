# Ansible Role: Apache2 mod_oauth2

Installs mod_oauth2 from source on any Debian/Ubuntu Linux system.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    libcurl4_ssl_variant: nss
    liboauth2_source_url: https://github.com/zmartzone/liboauth2
    liboauth2_source_dir: /usr/local/src/liboauth2
    liboauth2_source_version: v1.4.1
    liboauth2_source_user: root

    mod_oauth2_source_url: https://github.com/zmartzone/mod_oauth2
    mod_oauth2_source_dir: /usr/local/src/mod_oauth2
    mod_oauth2_source_version: v3.2.1
    mod_oauth2_source_user: root


## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
        - { role: tkanemoto.apache2-mod-oauth2 }

## License

MIT / BSD

## Author Information

This role was created in 2021 by [Takeshi Kanemoto](http://tkanemoto.com/).
