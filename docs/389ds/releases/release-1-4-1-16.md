---
title: "Releases/1.4.1.16"
---

389 Directory Server 1.4.1.16
-----------------------------

The 389 Directory Server team is proud to announce 389-ds-base version 1.4.1.16

Fedora packages are available on Fedora 30.

<https://koji.fedoraproject.org/koji/taskinfo?taskID=42539571> - Fedora 30

Bodhi

<https://bodhi.fedoraproject.org/updates/FEDORA-2020-b9e37ebd1e> - Fedora 30

The new packages and versions are:

- 389-ds-base-1.4.1.16-1

Source tarballs are available for download at [Download 389-ds-base Source](https://releases.pagure.org/389-ds-base/389-ds-base-1.4.1.16.tar.bz2)

### Highlights in 1.4.1.16

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

The new UI is complete, and fully ported to React JS


### Feedback

We are very interested in your feedback!

Please provide feedback and comments to the 389-users mailing list: <https://lists.fedoraproject.org/admin/lists/389-users.lists.fedoraproject.org>

If you find a bug, or would like to see a new feature, file it in our Pagure project: <https://pagure.io/389-ds-base>

- Bump version to 1.4.1.16
- Issue 50499 - Fix npm audit issues
- Issue 50884 - Health check tool DSEldif check fails
- Issue 50926 - Remove dual spinner and other UI fixes
- Issue 50928 - Unable to create a suffix with countryName
- Issue 50758 - Only Recommend bash-completion, not Require
- Issue 50904 - Connect All React Components And Refactor the Main Navigation Tab Code
- Issue 50919 - Backend delete fails using dsconf
- Issue 50872 - dsconf can't create GSSAPI replication agreements
- Issue 50914 - No error returned when adding an entry matching filters for a non existing automember group
- Issue 50909 - nsDS5ReplicaId cant be set to the old value it had before
- Issue 50898 - ldclt core dumped when run with -e genldif option


