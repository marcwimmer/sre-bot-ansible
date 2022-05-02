# Ansible SRE Bots (Site Reliability Bots)

## Configuration

```yaml

sre_bots:
  hosts:
    HOSTNAME
  vars:
    broker_ip: 127.0.0.1
    host_name: Srv-Mon02
    bots:
      - path1
      - path2
    pip:
      - sre-bot-slack
      - sre-bot-zabbix

    configs:
        - name: /etc/sre/zabbix.conf
        value: |
            {
            "url": "http://localhost:8888",
            "user": "Admin",
            "password": "*********"
            }

```