# arl.aws

Ansible collection for Amazon Linux 2.

## Usage

`requirements.yml`
```
collections:
  - source: git+https://github.com/ngyewch/ansible-collections.git
    version: v1.5.0
    type: git
``````

## Roles

## arl.aws.certbot

Install certbot.

### arl.aws.epel

Install [EPEL](https://docs.fedoraproject.org/en-US/epel/) repository.

## arl.aws.nginx

Install nginx.

## arl.aws.nginx_proxy

Set up nginx reverse proxy.

| Variable | Description |
| --- | --- |
| domain_name | Domain name. |
| proxy_pass | Upstream. |

## arl.aws.oauth2_proxy

Install oauth2-proxy.

## arl.aws.oauth2_proxy_service

Install oauth2-proxy service.

| Variable | Description |
| --- | --- |
| instance_name | Instance name. |

Templates:
* etc/oauth2-proxy/{{ instance_name }}.cfg

## arl.aws.ssl_cert

Request SSL cert from LetsEncrypt via certbot.

| Variable | Description |
| --- | --- |
| domain_name | Domain name. |
| email_address | Email address. |

## arl.aws.strongswan_server

Install Strongswan server.

Files:
* etc/strongswan/ipsec.conf.d/*
* etc/strongswan/ipsec.secrets.d/*

Templates:
* etc/strongswan/ipsec.conf.d/*
* etc/strongswan/ipsec.secrets.d/*
