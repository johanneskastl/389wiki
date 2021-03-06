---
title: "Releases/1.4.1.15"
---

389 Directory Server 1.4.1.15
-----------------------------

The 389 Directory Server team is proud to announce 389-ds-base version 1.4.1.15

Fedora packages are available on Fedora 30.

<https://koji.fedoraproject.org/koji/taskinfo?taskID=41482951> - Fedora 30

Bodhi

<https://bodhi.fedoraproject.org/updates/FEDORA-2020-9eb0691f9e> - Fedora 30

The new packages and versions are:

- 389-ds-base-1.4.1.15-1

Source tarballs are available for download at [Download 389-ds-base Source](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.1.15.tar.bz2)

### Highlights in 1.4.1.15

- Bug fixes

### Installation and Upgrade 

See [Download](../download.html) for information about setting up your yum repositories.

To install the server use **dnf install 389-ds-base**

To install the Cockpit UI plugin use **dnf install cockpit-389-ds**

After rpm install completes, run **dscreate interactive**

For upgrades, simply install the package.  There are no further steps required.

There are no upgrade steps besides installing the new rpms 

See [Install\_Guide](../howto/howto-install-389.html) for more information about the initial installation and setup

See [Source](../development/source.html) for information about source tarballs and SCM (git) access.

### New UI Progress (Cockpit plugin)

The new UI is fully functional.  There are still parts that need to be converted to ReactJS, but every feature is available.

|Configuration Tab|Functional|Written in ReactJS |
|-----------------|----------|-------------------|
|Server Tab       |Yes       |Yes                |
|Security Tab     |Yes       |Yes                |
|Database Tab     |Yes       |Yes                |
|Replication Tab  |Yes       |Yes                |
|Schema Tab       |Yes       |Yes                |
|Plugin Tab       |Yes       |Yes                |
|Monitor Tab      |Yes       |Yes                |
|Navigiation Bar  |Yes       |No                 |


### Feedback

We are very interested in your feedback!

Please provide feedback and comments to the 389-users mailing list: <https://lists.fedoraproject.org/admin/lists/389-users.lists.fedoraproject.org>

If you find a bug, or would like to see a new feature, file it in our Pagure project: <https://pagure.io/389-ds-base>

- Bump version to 1.4.1.15
- Issue 50855 - remove unused file from UI
- Issue 50855 - UI: Port Server Tab to React
- Issue 50636 - Crash during sasl bind
- Issue 49623 - cenotaph errors on modrdn operations (part 2)
- Issue 50882 - Fix healthcheck errors for instances that do not have TLS enabled
- Issue 50886 - Typo in the replication debug message
- Issue 50873 - Fix healthcheck and virtual attr check
- Issue 50873 - Fix issues with healthcheck tool
- Issue 50857 - Memory leak in ACI using IP subject
- Issue 49624 - DB Deadlock on modrdn appears to corrupt database and entry cache (part 2)
- Issue 50823 - dsctl doesn't work with 'slapd-' in the instance name
- Issue 50824 - dsctl remove fails with "name 'ensure_str' is not defined"
- Issue 50798 - incorrect bytes in format string(fix import issue)
- Issue 50798 - incorrect bytes in format string
- Issue 50850 - Fix dsctl healthcheck for python36
- Issue 49990 - Need to enforce a hard maximum limit for file descriptors


