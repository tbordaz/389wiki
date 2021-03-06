---
title: "Releases/1.3.8.2"
---

389 Directory Server 1.3.8.2
-----------------------------

The 389 Directory Server team is proud to announce 389-ds-base version 1.3.8.2

Fedora packages are available on Fedora 27.

<https://koji.fedoraproject.org/koji/taskinfo?taskID=27171470>

<https://bodhi.fedoraproject.org/updates/FEDORA-2018-f440642085>

The new packages and versions are:

-   389-ds-base-1.3.8.2-1

Source tarballs are available for download at [Download 389-ds-base Source](https://releases.pagure.org/389-ds-base/389-ds-base-1.3.8.2.tar.bz2)

### Highlights in 1.3.8.2

- Security and bug fixes

### Installation and Upgrade 
See [Download](../download.html) for information about setting up your yum repositories.

To install, use **yum install 389-ds** yum install 389-ds After install completes, run **setup-ds-admin.pl** if you have 389-admin installed, otherwise please run **setup-ds.pl** to set up your directory server.

To upgrade, use **yum upgrade** yum upgrade After upgrade completes, run **setup-ds-admin.pl -u** if you have 389-admin installed, otherwise please run **setup-ds.pl** to update your directory server/admin server/console information.

See [Install\_Guide](../legacy/install-guide.html) for more information about the initial installation, setup, and upgrade

See [Source](../development/source.html) for information about source tarballs and SCM (git) access.

### Feedback

We are very interested in your feedback!

Please provide feedback and comments to the 389-users mailing list: <https://lists.fedoraproject.org/admin/lists/389-users.lists.fedoraproject.org>

If you find a bug, or would like to see a new feature, file it in our Pagure project: <https://pagure.io/389-ds-base>

- Bump version to 1.3.8.2
- Ticket 48184 - clean up and delete connections at shutdown (2nd try)
- Ticket 49696 - replicated operations should be serialized
- Ticket 49671 - Readonly replicas should not write internal ops to changelog
- Ticket 49665 - Upgrade script doesn't enable CRYPT password storage plug-in
- Ticket 49665 - Upgrade script doesn't enable PBKDF2 password storage plug-in

