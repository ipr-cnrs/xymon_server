# Xymon Server

1. [Overview](#overview)
2. [Role Variables](#role-variables)
3. [Example Playbook](#example-playbook)
4. [Configuration](#configuration)
5. [Development](#development)
6. [License](#license)
7. [Author Information](#author-information)

## Overview

Manage Xymon server installation and configuration.

## Role Variables

* **xymon_server__base_packages** : List of base packages in order to provide `xymon` server [default : `xymon`].
* **xymon_server__deploy_state** : The desired state this role should achieve [default : `present`].
* **ymon_server__etc_src** : Directory used as source to templating /etc configuration content [default : `etc/xymon`].

## Example Playbook

* Use defaults vars :

``` yml
- hosts: serverXYZ
  roles:
    - role: ipr-cnrs.xymon_server
```

## Configuration

This role will :
* Install needed packages to provide `xymon` server.
* Manage `xymon` server configuration (/etc).

## Development

This source code comes from our [Gogs instance][xymon_server source] and the [Github repo][xymon_server github] exist just to be able to send the role to Ansible Galaxy…

But feel free to send issue/PR here :)

Thanks to this [hook][gogs to github hook], Github automatically got updates from our [Gogs instance][xymon_server source] :)

## License

[WTFPL][wtfpl website]

## Author Information

Jérémy Gardais
* Source : [on IPR's Gogs][xymon_server source]
* [IPR][ipr website] (Institut de Physique de Rennes)

[gogs to github hook]: https://stackoverflow.com/a/21998477
[xymon_server source]: https://git.ipr.univ-rennes1.fr/cellinfo/ansible.xymon_server
[xymon_server github]: https://github.com/ipr-cnrs/xymon_server
[wtfpl website]: http://www.wtfpl.net/about/
[ipr website]: https://ipr.univ-rennes1.fr/
