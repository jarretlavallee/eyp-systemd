# CHANGELOG

## 0.1.28

* addded KillMode to **systemd::service**

## 0.1.27

* added standard_error and standard_output variables to **systemd::service** (default to syslog, keeping compatibility)

## 0.1.26

* added ExecStartPost options to **systemd::service**
* allow multiple commands for **ExecStart** and **ExecStop** (besed on [PR-32](https://github.com/NTTCom-MS/eyp-systemd/pull/32))

## 0.1.25

* added minimal socket support

## 0.1.24

* acceptance testing skeleton

## 0.1.23

* Added StartLimitInterval and StartLimitBurst - thanks to [steveniemitz](https://github.com/steveniemitz) for this PR
* Fixed UMask casing and removed redundant default - thanks to [steveniemitz](https://github.com/steveniemitz) for this PR

## 0.1.22

* added to **systemd::service**
  * environment_files - thanks to [oOHenry](https://github.com/oOHenry) for this PR
  * umask
  * nice
  * oom_score_adjust

## 0.1.21

* added SLES12 support
* added to **systemd::service**:
  * working_directory
  * root_directory

## 0.1.20

* added to **systemd::service**:
  * restart_sec
  * private_tmp
  * limit_nproc
  * limit_nice
* enhanced restart validation

## 0.1.19

* added service variables:
  * permissions_start_only
  * execstartpre
  * timeoutstartsec
  * timeoutstopsec
  * timeoutsec
  * restart_prevent_exit_status
  * limit_nofile
  * runtime_directory
  * runtime_directory_mode

## 0.1.18

* added service ordering variables:
  * wants
  * before
  * after
  * requires
  * conflicts
* added **wantedby** and **requiredby**

## 0.1.17

* added **env_vars** - thanks to [dzmitryv](https://github.com/dzmitryv) for this PR
* added options:
  * after
  * remain_after_exit
  * type
  * execreload

## 0.1.16

* added description
* added Ubuntu 16.04

## 0.1.14

* added **eyp_systemd_available** fact
* added configurable check time for sysv wrapper

## 0.1.12

* added sysvwrapper for sysv init scripts without PIDFILE

## 0.1.11

*  pidfile for systemd::service

## 0.1.10

* support for Ubuntu 16.04 and Debian 8
