# kibana

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/kibana) [![Testing Build](https://github.com/rolehippie/kibana/workflows/testing/badge.svg)](https://github.com/rolehippie/kibana/actions?query=workflow%3Atesting) [![Readme Build](https://github.com/rolehippie/kibana/workflows/readme/badge.svg)](https://github.com/rolehippie/kibana/actions?query=workflow%3Areadme) [![Galaxy Build](https://github.com/rolehippie/kibana/workflows/galaxy/badge.svg)](https://github.com/rolehippie/kibana/actions?query=workflow%3Agalaxy) [![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/kibana)](https://github.com/rolehippie/kibana/blob/master/LICENSE)

Ansible role to install and configure a Kibana dashboard.

## Sponsor

[![Proact Deutschland GmbH](https://proact.eu/wp-content/uploads/2020/03/proact-logo.png)](https://proact.eu)

Building and improving this Ansible role have been sponsored by my employer **Proact Deutschland GmbH**.

## Table of content

- [Default Variables](#default-variables)
  - [kibana_elasticsearch_hosts](#kibana_elasticsearch_hosts)
  - [kibana_elasticsearch_preserve_host](#kibana_elasticsearch_preserve_host)
  - [kibana_group](#kibana_group)
  - [kibana_repository](#kibana_repository)
  - [kibana_server_base_path](#kibana_server_base_path)
  - [kibana_server_name](#kibana_server_name)
  - [kibana_server_version](#kibana_server_version)
  - [kibana_user](#kibana_user)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### kibana_elasticsearch_hosts

#### Default value

```YAML
kibana_elasticsearch_hosts: []
```

### kibana_elasticsearch_preserve_host

#### Default value

```YAML
kibana_elasticsearch_preserve_host: false
```

### kibana_group

Name of the group owning Kibana

#### Default value

```YAML
kibana_group: kibana
```

### kibana_repository

Dict of repositories matching the choosen version

#### Default value

```YAML
kibana_repository:
  '7.8': deb https://artifacts.elastic.co/packages/7.x/apt stable main
```

### kibana_server_base_path

When this setting's value is true Kibana uses the hostname specified in server host

### kibana_server_name

Name of the server

#### Default value

```YAML
kibana_server_name: '{{ ansible_hostname }}'
```

### kibana_server_version

Version of Logstash that gets installed

#### Default value

```YAML
kibana_server_version: '7.8'
```

### kibana_user

Name of the user owning Kibana

#### Default value

```YAML
kibana_user: kibana
```

## Discovered Tags

**_kibana_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
