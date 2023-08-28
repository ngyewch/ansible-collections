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

### arl.aws.epel

Install [EPEL](https://docs.fedoraproject.org/en-US/epel/) repository.

## arl.aws.nginx

Install nginx.

## arl.aws.certbot

Install certbot.

## arl.aws.ssl_cert

Request SSL cert from LetsEncrypt via certbot.

| Variable | Description |
| --- | --- |
| domain_name | Domain name. |
| email_address | Email address. |
