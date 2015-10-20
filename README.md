ansible-role-influxdb
=========

Provision a basic influxDB instance. Can optionally install Grafana and/or Chronograf on the same box. Works well for development environments.

Role Variables
--------------



    influxdb_bind_address: "0.0.0.0"
    influxdb_host: "{{ influxdb_bind_address }}"
    influxdb_port: 8086
    influxdb_user: "default_user"
    influxdb_password: "passw0rd"
    influxdb_version: 0.9.4.2
    influxdb_grafana_password: "passw0rd"
    influxdb_root_password: "passw0rd"

    chronograf_version: "0.2.0"
    install_chronograf: false

    grafana_version: "2.1.3"
    install_grafana: true


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: influxdb
      sudo: True
      roles:
        - ansible-role-influxdb

License
-------

MIT

Author Information
------------------

optimuspaul
