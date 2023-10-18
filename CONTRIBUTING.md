Contributing to Mender
======================

Thank you for showing interest in contributing to the Mender project.
Connecting with contributors and growing a community is very important to us.
We hope you will find what you need to get started on this page.

## Contribution coordination during client rewrite to C++

We have announced a [rewrite of substantial client parts to C++](https://hub.mender.io/t/mender-to-rewrite-client-using-c-and-retain-go-for-its-backend/5332/1). As this rewrite must
provide feature parity to the current go implementation, contributions need to follow a few
guidelines while the rewrite is in progress.

- Bug and security fixes are acceptable and welcome for the go client. Please see the
following paragraphs for more details.
- Feature additions are only acceptable for the [rewrite branch](https://github.com/mendersoftware/mender/tree/feature-c++-client). As this branch is under
heavy development at the moment, is is highly advisable to coordinate with the development
team on the [Mender Hub](https://github.com/mendersoftware/mender/tree/feature-c++-client).

## Reporting security issues

If you come across any security issue, please bring it to our team's
attention as quickly as possible by sending an email to
[security@mender.io](mailto:security@mender.io).

Please do not disclose anything in public. Once an issue has been addressed we
will publish the fix and acknowledge your finding on our site if you so wish.


## Proposed tasks to get started

There is a `helpwanted` tag on some tasks in the Mender issue tracker
that have been identified as good candidates for initial contributors.

You can see them in the [Help Wanted saved filter](https://northerntech.atlassian.net/issues/?filter=10084).


## Providing pull requests

Pull requests are very welcome, and the maintainers of Mender work hard
to stay on top to review and hopefully merge your work.

If your work is significant, it can make sense to discuss the idea with the
maintainers and relevant project members upfront. Start a discussion on our [Mender Hub forum](https://hub.mender.io/c/general-discussions).

Using commit signoffs tags is mandatory for all commits; we also
encourage that each commit is small and cohesive. See the next sections for details.


### Sign your work

Mender is licensed under the Apache License, Version 2.0. To ensure open source
license compatibility, we need to keep track of the origin of all commits and
make sure they comply with the license. To do this, we follow the same procedure
as used by the Linux kernel, and ask every commit to be signed off.

The sign-off is a simple line at the end of the explanation for the patch, which
certifies that you wrote it or otherwise have the right to pass it on as an
open-source commit.  The rules are pretty simple: if you can certify the below
(from [developercertificate.org](http://developercertificate.org/)):


```
Developer Certificate of Origin
Version 1.1

Copyright (C) 2004, 2006 The Linux Foundation and its contributors.
660 York Street, Suite 102,
San Francisco, CA 94110 USA

Everyone is permitted to copy and distribute verbatim copies of this
license document, but changing it is not allowed.

Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the best
    of my knowledge, is covered under an appropriate open source
    license and I have the right under that license to submit that
    work with modifications, whether created in whole or in part
    by me, under the same open source license (unless I am
    permitted to submit under a different license), as indicated
    in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including all
    personal information I submit with it, including my sign-off) is
    maintained indefinitely and may be redistributed consistent with
    this project or the open source license(s) involved.
```

Then you just add a line to every git commit message:

    Signed-off-by: Random J Developer <random@developer.example.org>

Use your real name (sorry, no pseudonyms or anonymous contributions).

If you set your `user.name` and `user.email` git configs, you can sign your
commit automatically with `git commit -s`.


### Structuring your commits

More often than not, your pull request will come as a set of commits, not just
a single one. This is especially recommended in case of larger changesets.

In that case, please make sure that each commit constitutes a cohesive, logical
whole, e.g.  modifies a given package, function, or application layer. There are many ways
to conceptually divide your changeset, depending on its size and content - this is up to you.
It's just important that unrelated changes are not mixed up together in unrelated commits.

This is to ensure that:
* your PR is easy to browse and review
* git log is easier to digest

At the Mender project we are adhering to a slightly modified version of
[conventional
commits](https://www.conventionalcommits.org/en/v1.0.0/#specification). The full
specification of which can be found
[here](https://github.com/mendersoftware/mendertesting/blob/master/commitlint/grammar.md).

tldr; in general your contribution will fall into one of two categories:

1. A fix

In this case, structure your commit like below:

```
fix: <description of the fix>

<More detailed explanation of the commit>

Changelog: <None|Title|Commit|All>
Ticket: <None|Ticket Nr>
```



* A new feature

```
feat: <description of the new feature>

<More detailed explanation of the commit>

Changelog: <None|Title|Commit|All>
Ticket: <None|Ticket Nr>
```

## Contributor Code of Conduct

We have a [Code of Conduct](https://github.com/mendersoftware/mender/blob/master/code-of-conduct.md) that applies to all contributors and participants to the Mender project.


## Let us work together with you

In an ever more digitized world, securing the world's connected devices is a
very important and meaningful task. To succeed, we will need to row in the same
direction and work to the best interest of the project.

This project appreciates your friendliness, transparency and a collaborative
spirit.
