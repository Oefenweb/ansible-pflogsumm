## pflogsumm

[![Build Status](https://travis-ci.org/Oefenweb/ansible-pflogsumm.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-pflogsumm) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-pflogsumm-blue.svg)](https://galaxy.ansible.com/list#/roles/1687)

Set up pflogsumm in Debian-like systems.

#### Requirements

* `formail` (will be installed)

#### Variables

* `pflogsumm_report_from` [default: `pflogsumm`]: The mail address reports are sent from
* `pflogsumm_report_to` [default: `root`]: The mail address reports are sent to
* `pflogsumm_report_subject` [default: ``'[pflogsumm] `hostname -f`: mail statistics'``]: The subject line for the report mails
* `pflogsumm_logrotate_interval` [default: `daily`]: Log files are rotated every <interval>.
* `pflogsumm_logrotate_times` [default: `7`]: Log files are rotated <times> times before being removed

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
    - pflogsumm
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-pflogsumm/issues)!
