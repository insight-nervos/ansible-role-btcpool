ansible-role-btcpool
=========

Configures a node to run a dockerized version of btcpool v1 with plans to update to the new v2 spec as the project progresses. 

Requirements
------------

Ubuntu 18.04+.  Best used with the associated terraform modules which wrap the call of this module. 

- [AWS terraform module](https://github.com/insight-stratum/terraform-btcpool-aws-node)
- [Alibaba terraform module](https://github.com/insight-stratum/terraform-btcpool-alibaba-network)

Role Variables
--------------

> WIP

Dependencies
------------

- [certbot](https://github.com/geerlingguy/ansible-role-certbot)

Example Playbook
----------------

`requirements.yaml` -> `ansible-galaxy install -r requirements.yml`
```yaml
roles:
  - src: insight_nervos.btcpool
```

Playbook:
```yaml
- hosts: all
  roles:
    - insight_nervos.btcpool
```

License
-------

Apache 2.0
