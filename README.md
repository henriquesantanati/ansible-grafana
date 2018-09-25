ansible-grafana
=========

Installation and configuration of Grafana Server using Ansible with LDAP integration and Zabbix Plugin.

Requirements
------------

Ansible for play the role.
CentOS or RedHat Server

Role Variables
--------------
```yml
{
  grafana_rpm - path of RPM file. Should be a local webserver (without internet connection).
  grafana_ini - path of ini file
  grafana_ldap_config - path of LDAP config for AD integration
  grafana_ldap_user - user for bind LDAP
  grafana_ldap_pwd - password for LDAP user
  grafana_ldap_server - AD Server
  grafana_ldap_admin_grp - Group for restriction
  grafana_ldap_grpsearch - OU for search
  grafana_http_port - Grafana port. Default 3000 but in the role we will set for default HTTP port (80)
  grafana_http_domain - domain for url
}
```

Dependencies
------------

None ;)
