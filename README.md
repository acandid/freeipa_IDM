FreeIPA/IDM
===========

Install and configuring FreeIPA/IDM on Rocky Linux

- Install the necessary packages;
- Configure ipa-server and ipa-client

Requirements
------------

- The SELinux and firewall settings are not considered to be a concern of this role.

Role Variables
--------------

Necessary changes to defaults/main.yml

| Variables                                    | Defaults                      | Comments
| :---                                         | :---                          | :---                                                    
| `freeipa_IDM_domain`                         |                               | Inform your domain
|                                              |                               |
| `freeipa_IDM_realm`                          |                               | Inform your realm
|                                              |                               |
| `freeipa_IDM_ds_password`                    |                               | Inform DS password
|                                              |                               |
| `freeipa_IDM_admin_password`                 |                               | Inform admin password
|                                              |                               |
| `freeipa_IDM_ipa_admin`                      | admin                         | Inform admin user
|                                              |                               | 



Read with Attention!
====================

You need to have prior knowledge of FreeIPA/IDM to understand what's going on and make the necessary changes to suit your needs.
--------------------------------------------------------------------------------------------------------------------------------

Was using /etc/hosts file because I don't have DNS structure in my test environment, IPA will be configured to be used as DNS server. If you have a DNS server in your structure, you must make the necessary changes.


Dependencies
------------

No dependencies.

The Inventory should be created as below the group name should be kept.
-----------------------------------------------------------------------
```
[ipaserver]
freeipa01.almircandidorocky.com

[ipareplica]
freeipa02.almircandidorocky.com

[ipaclient]
client01.almircandidorocky.com

```


## Contributing

Issues, feature requests, ideas are appreciated and can be posted in the Issues section.


Author Information
------------------
LinkedIn: https://br.linkedin.com/in/almircandido/
