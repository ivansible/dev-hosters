# ivansible.dev_hosters

[![Github Test Status](https://github.com/ivansible/dev-hosters/workflows/test/badge.svg?branch=master)](https://github.com/ivansible/dev-hosters/actions)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-ivansible.dev__hosters-68a.svg?style=flat)](https://galaxy.ansible.com/ivansible/dev_hosters/)

Install CLI for Amazon AWS, Azure, DigitalOcean, Heroku, Packet, Vultr.

Installation instructions:
- AWS:  https://docs.aws.amazon.com/cli/latest/userguide/awscli-install-linux.html
- AWless:  https://github.com/wallix/awless/wiki/Installation
- Azure:  https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-apt
- DigitalOcean:  https://github.com/digitalocean/doctl#installing-doctl
- Heroku:  https://devcenter.heroku.com/articles/heroku-cli#ubuntu-debian-apt-get
- Packet: https://github.com/ebsarr/packet
- Vultr:  https://github.com/JamesClonk/vultr#installation


## Requirements

None


## Variables

    devhost_upgrade: false
Allows to upgrade already installed packages.

    devhost_digitalocean_token: ""
API token for DigitalOcean (only eligible for `permitted` host group).

    devhost_packet_auth_token: ""
    devhost_packet_default_project: ""
API token and project Id for Packet (only eligible for `permitted` host group).


## Tags

- `devhost_aws`
- `devhost_awless`
- `devhost_azure`
- `devhost_digitalocean`
- `devhost_heroku`
- `devhost_packet`
- `devhost_vultr`
- `devhost_all`


## Dependencies

- `ivansible.lin_base`
- `ivansible.lin_go` (for Packet cli, imports `lin_go_version`)


## Example Playbook

    - hosts: devhost
      roles:
        - ivansible.dev_hosters


## License

MIT


## Author Information

Created in 2018-2021 by [IvanSible](https://github.com/ivansible)
