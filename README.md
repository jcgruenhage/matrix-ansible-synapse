matrix-synapse
==============

Install a matrix synapse server.

Requirements
------------

The following should be present on the target system
* `pip`
* `systemd`
* `rsyslogd`
* `logrotate`

Role Variables
--------------

__Default vars__

| Name | Value |
| :--- | :---  |
| matrix_synapse_tls_path | "/opt/synapse/ssl/{{ matrix_synapse_domain }}.crt" |
| matrix_synapse_key_path | "/opt/synapse/ssl/{{ matrix_synapse_domain }}.key" |
| matrix_synapse_dh_path | "/opt/synapse/ssl/{{ matrix_synapse_domain }}.dh" |
| matrix_synapse_server_name | "{{ matrix_synapse_domain }}" |
| matrix_synapse_baseurl | "https://{{ matrix_synapse_domain }}" |
| matrix_synapse_port_prefix | 100 |
| matrix_synapse_pg_pass | "{{ matrix_pg_pass }}" | 
| matrix_synapse_pg_user | "{{ matrix_pg_user }}" |
| matrix_synapse_pg_db | "{{ matrix_pg_db }}" |
| matrix_synapse_pg_host | "{{ matrix_pg_host }}" |
| matrix_synapse_log_config | "/opt/synapse/{{ matrix_synapse_domain }}.log.config" |
| matrix_synapse_media_store_path | "/opt/synapse/media_store" |
| matrix_synapse_uploads_path | "/opt/synapse/uploads" |
| matrix_synapse_turn_secret | "{{ matrix_turn_secret }}" |
| matrix_synapse_turn_uri | "{{ matrix_turn_uri }}" |
| matrix_synapse_registration_secret | "{{ matrix_registration_secret }}" |
| matrix_synapse_macaroon_secret_key | "{{ matrix_macaroon_key }}" |
| matrix_synapse_signing_key_path | "/opt/synapse/ssl/{{ matrix_synapse_domain }}.signing.key" |
| matrix_synapse_version | "v0.28.1" |
| matrix_synapse_log_days_keep | 30 |
| matrix_synapse_skip_ssl | false |

Dependencies
------------

__None__.

Example Playbook
----------------

```yaml
#TODO: Add example
```

License
-------

Apache 2.0

Author Information
------------------

* Michael Kaye
* Jan Christian Grünhage
* Emmanouil Kampitakis
