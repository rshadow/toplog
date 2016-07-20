# toplog
Script to search periodical critical load average on servers. Save most used info to log file.

## Install

* Clone
* Install `top` and `iotop` packages.
* Add `top_log` to crontab every minutes
* Copy `logrotate.d/top_log` to `/etc/logrotate.d`

## Usage

Just analyze `/var/log/top.log` for critical load average.

For example you can find all big digits:

```
  grep "[1-9][0-9]+" /var/log/top.log
```
