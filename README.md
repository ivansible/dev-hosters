# Role ivansible.lin-hosters

Install CLI for Amazon AWS, Azure, DigitalOcean, Heroku, Vultr.

Installation instructions:
- AWS:  https://docs.aws.amazon.com/cli/latest/userguide/awscli-install-linux.html
- Azure:  https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-apt
- DigitalOcean:  https://github.com/digitalocean/doctl#installing-doctl
- Heroku:  https://devcenter.heroku.com/articles/heroku-cli#ubuntu-debian-apt-get
- Vultr:  https://github.com/JamesClonk/vultr#installation


## Requirements

None


## Variables

    linhost_allow_reinstall: no

Allows to refresh already downloaded redistributables.

    linhost_doctl_token: ''

API token for DigitalOcean (only eligible for `workspace` group).


## Tags

- `linhost_aws`
- `linhost_azure`
- `linhost_do`
- `linhost_heroku`
- `linhost_vultr`


## Dependencies

None


## Example Playbook

    - hosts: vag2
      roles:
        - role: ivansible.lin-hosters


## License

MIT


## Author Information

Created in 2018 by [IvanSible](https://github.com/ivansible)
