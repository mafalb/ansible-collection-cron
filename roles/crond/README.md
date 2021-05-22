# Ansible Role mafalb.cron.crond

Ansible role mafalb.cron.crond

## Basic Usage

```yaml
- name: anacron is present
  hosts: localhost
  roles:
  - role: mafalb.cron.crond
    anacron: true
```

```yaml
- name: both cron and anacron is absent
  hosts: localhost
  roles:
  - role: mafalb.cron.crond
    state: absent
```

```yaml
- name: only cron is installed, not anacron
  hosts: localhost
  roles:
  - role: mafalb.cron.crond
    anacron: false
```

## Variables

---

### anacron

Install anacron or not

```yaml
anacron: true
```

---

### state

cron is present or not

```yaml
state: present
```

---

## License

Copyright (c) 2020,2021 Markus Falb <markus.falb@mafalb.at>

GPL-3.0-or-later
