# ivansible.dev_hosters

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

    devhost_allow_reinstall: no

Allows to refresh already downloaded redistributables.

    devhost_digitalocean_token: ""

API token for DigitalOcean (only eligible for `permitted` host group).


## Tags

- `devhost_aws`
- `devhost_azure`
- `devhost_do`
- `devhost_heroku`
- `devhost_vultr`


## Dependencies

None


## Example Playbook

    - hosts: vag2
      roles:
        - role: ivansible.dev_hosters


## License

MIT


## Author Information

Created in 2018 by [IvanSible](https://github.com/ivansible)
