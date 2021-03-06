---
title: Development Page
---

# 389 Directory Server Development
----------------------------------

{% include toc.md %}

Directory Server is huge! Where do I even start?
------------------------------------------------

The best way to start is not to try and write code straight up. Install a Directory Server instance, and use it. Join our users list and ask questions - We are nice people, no question is bad (read our archives if you don't believe me).

As you use a piece of software, you'll start to see rough edges, things that could be better, even ways you wish you could use it differently. Talk to us, and see if you could help by giving us ideas, or even writing it yourself. We'll help guide you in the process. Raising a bug is just as important as the potential to write a fix.

Many of us in the team started by asking questions and raising bugs - Not by jumping in the deep end with patches.

Developer's
-----------

Developers should check out our [building](development/building.html) and [install](legacy/install-guide.html) guides to see how to build and install the server from source. Then you can get working on fixing [bugs](FAQ/bugs.html), adding new [features](FAQ/features.html), adding new test cases to [lib389 Continuous Integration](FAQ/upstream-test-framework.html), or improving our [documentation](documentation.html).  For other ideas see [ways to contribute](FAQ/ways-to-contribute.html).

To browse through our backlog of development tickets, access the [389 Trac instance](FAQ/bugs.html). The team can help advise you on the potential complexity or simpliticy of any issue want to attempt.

If you want to contribute code to the project you should look at our ICLA on this page. It contains information on the process you have to go through to be able to submit patches we will accept as well as getting a git. From a more technical standpoint, before submitting a patch you should check out our [coding style](development/coding-style.html) guide. Once your patch is approved, see the [Git rules](development/git-rules.html) before checking anything in.

Please take some time to review our [license](FAQ/licensing.html).


Guidelines
------------
-   [Coding Style](development/coding-style.html)
-   [Git Rules](development/git-rules.html) - rules and guidelines for submitting patches and pushing to upstream
-   [Git information](http://git-scm.com/)
    -   [Official Git tutorial](http://www.kernel.org/pub/software/scm/git/docs/gittutorial.html)
    -   [Everyday Git](http://www.kernel.org/pub/software/scm/git/docs/everyday.html) - day to day usage examples for different roles
    -   [Git Users Manual](http://www.kernel.org/pub/software/scm/git/docs/user-manual.html)
    -   [Reference Manual](http://www.kernel.org/pub/software/scm/git/docs/) - man pages
    -   [Git Community Book](http://book.git-scm.com/)
    -   [Git Visual Cheat Sheet](http://zrusin.blogspot.com/2007/09/git-cheat-sheet.html)
    -   [Linus Torvalds on Git](http://www.youtube.com/watch?v=4XpnKHJAok8)
-   [How to Build RPMS on CentOS ](howto/howto-buildrpmsforcentos-rhel.html)


<a name="source"></a>

Source Code and Build Instructions
--------------------------------------------------------

**[Download Source Code - Click Here](development/source.html)**

|Component|GIT Repository|Clone the Repository|
|---------|------|
|**Directory Server** ([build & debug instructions](development/building.html))| <https://git@pagure.io/389-ds-base.git>| git clone https://git@pagure.io/389-ds-base.git<br>git clone ssh://git@pagure.io/389-ds-base.git|
|**Nunc-Stans** ([build & debug instructions](development/building-nunc-stans.html))| <https://git.fedorahosted.org/git/nunc-stans.git>| git clone git://git.fedorahosted.org/git/nunc-stans.git<br>git clone ssh://git.fedorahosted.org/git/nunc-stans.git|
|**AdminUtil** ([build instructions](administration/adminutil.html)) | <https://git.fedorahosted.org/git/389/adminutil.git>| git clone git://git.fedorahosted.org/git/389/adminutil.git<br>git clone ssh://git.fedorahosted.org/git/389/adminutil.git|
|**Admin Server** ([build & debug instructions](administration/adminserver.html#build)) | <https://git.fedorahosted.org/git/389/admin.git>| git clone git://git.fedorahosted.org/git/389/admin.git<br>git clone ssh://git.fedorahosted.org/git/389/admin.git|
|**IDM Console Framework** ([build & debug instructions](development/buildingconsole.html#framework)) | <https://git.fedorahosted.org/git/idm-console-framework.git>| git clone git://git.fedorahosted.org/git/idm-console-framework.git<br>git clone ssh://git.fedorahosted.org/git/idm-console-framework.git|
|**389 Console** ([build & debug instructions](development/buildingconsole.html#console)) | <https://git.fedorahosted.org/git/389/console.git>| git clone git://git.fedorahosted.org/git/389/console.git<br>git clone ssh://git.fedorahosted.org/git/389/console.git|
|**DS Console** ([build & debug instructions](development/buildingconsole.html#ds-console)) | <https://git.fedorahosted.org/git/389/ds-console.git>| git clone git://git.fedorahosted.org/git/389/ds-console.git<br>git clone ssh://git.fedorahosted.org/git/389/ds-console.git|
|**Admin Console** ([build & debug instructions](development/buildingconsole.html#admin-console)) | <https://git.fedorahosted.org/git/389/admin-console.git>| git clone git://git.fedorahosted.org/git/389/admin-console.git<br>git clone ssh://git.fedorahosted.org/git/389/admin-console.git|
|**DSGW & Web Apps** ([build instructions](administration/dsgw-building.html)) | <https://git.fedorahosted.org/git/389/dsgw.git>| git clone git://https://git.fedorahosted.org/git/389/dsgw.git<br>git clone ssh://https://git.fedorahosted.org/git/389/dsgw.git|
|**DSML Gateway** ([build instructions](administration/dsml-gateway-building.html)) | <https://git.fedorahosted.org/git/389/dsmlgw.git>| git clone git://git.fedorahosted.org/git/389/dsmlgw.git<br>git clone ssh://git.fedorahosted.org/git/389/dsmlgw.git|
|**Passync/Winsync** ([build instructions](development/buildingpasssync.html)) | <https://git.fedorahosted.org/git/389/winsync.git>| git clone git://git.fedorahosted.org/git/389/winsync.git<br>git clone ssh://git.fedorahosted.org/git/389/winsync.git|
|**Continuous Integration Testing** ([documentation](FAQ/upstream-test-framework.html))| <https://git.fedorahosted.org/git/389/lib389.git>| git clone git://git.fedorahosted.org/git/389/lib389.git<br>git clone ssh://git.fedorahosted.org/git/389/lib389.git|
|**Rest Server** ([documentation](design/ldap-rest-api.html))| <https://git.fedorahosted.org/git/389/rest389.git>| git clone git://git.fedorahosted.org/git/389/rest389.git<br>git clone ssh://git.fedorahosted.org/git/389/rest389.git|
|**OpenLDAP** ([build instructions](development/building-openldap.html))|Not Available| git clone git://git.openldap.org/openldap.git|
|**Svrcore** ([build instructions](development/building-svrcore.html))|<https://pagure.io/svrcore.git>| git clone https://pagure.io/svrcore.git|

<br>

[Design Documents](design/design.html)
----------------

Feature design documents describing the various features that were introduced with each release of **389-ds-base** and **389-admin** are located at the **[Feature Design Documents](design/design.html)** page.

FHS style packaging
-------------------

389 can be built to use FHS style, /opt FHS style, or user specified prefix - see [FHS Packaging](development/fhs-packaging.html)

Directory Server Plugins
------------------------

It is possible to write plugins that allow you to extend the functionality of the Directory Server. Our [plugins](design/plugins.html) page contains information on the API and the scope of the functionality. You might also want to look at our [annotated license](FAQ/annotated-gpl-exception-license.html) page for some legal information on using the plugin api.

Release Engineering
-------------------

[Release Procedure](development/release-procedure.html)

Nightly Builds
--------------

[Nightly Builds](development/nightly-builds.html)

Testing
-------

Not a coder? No problem. You can help by finding new [bugs](FAQ/bugs.html), verifying existing bugs, polishing [documentation](documentation.html) and generally improving the quality of the server.

A good way to contribute to improving the quality of the server would be to add automated tests for each of the features. Developers and contributors to the 389 Project are encouraged to write unit tests for any new features, updates and bug fixes being contributed. Where possible, the tests should be data driven. This allows for greater numbers of test cases covering more of the feature under test, to be written with minimal effort. We suggest tests be written in a scripting language like python with lib389.

There are a number of other LDAP test tools available from other groups and companies which may be of interest:

-   [LDCLT](https://git.fedorahosted.org/cgit/389/ds.git/plain/ldap/servers/slapd/tools/ldclt/examples/README) The project maintained LDAP load testing tool.
-   [DirectoryMark](http://www.mindcraft.com/directorymark) from Mindcraft, is an LDAP benchmarking tool
-   [Slamd](http://www.slamd.com/) is a distributed LDAP load generation engine
-   [Using SystemTap](howto/howto-use-systemtap.html) - an example of using SystemTap to profile thread contention

If you know python, you can add to the *Continuous Integration Testing Framework (lib389)*, and help make the product more stable, and have less regressions in new releases.

-    [Upstream Testing Framework](FAQ/upstream-test-framework.html)

What can you do?
----------------

-   [Write a Wiki Page](howto/howto-write-wiki-page.html)
-   [Roadmap](FAQ/roadmap.html)
-   Timelines
-   [Wishlist](FAQ/wishlist.html)
-   [History](FAQ/history.html)
-   [File Bugs](FAQ/bugs.html)

Contributors
------------

-   [Mailing Lists, IRC](mailing-lists.html)
-   [389 Trac instance](FAQ/bugs.html)
-   Players (people involved)

Contributor License Agreement
-----------------------------

If you want to submit code and patches you need to sign the Fedora [Individual Contributor License Agreement](individual-contributor-license-agreement.html).

### Individual Contributor License Agreement

This is easy to do. Just follow these steps:

-   Go to <https://admin.fedoraproject.org/accounts/user/new> and create a new account - or Login if you already have an account
-   Go to <https://admin.fedoraproject.org/accounts/cla/> and submit the on-line form
    -   Some older versions of this text say that you have to print out, sign, and mail/fax/email the form. This is no longer a requirement for the ICLA - the click through is sufficient for the ICLA.



