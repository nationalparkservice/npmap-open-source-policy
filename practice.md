## Practicing our open source policy

This document is meant to give specific team guidance on putting our [open source policy](policy.md) into practice.

* NPMap releases software into the [international public domain](#public-domain).
* All team members should feel empowered to contribute back to outside open source projects.
* We [develop our software in the open](#working-in-public).
* There are [narrow, documented exceptions](#exceptions) where source code may be delayed or withheld.

NPMap team members should work with the strong presumption that all of their code will be public, throughout and after development.

Before deciding to delay or withhold the release of source code, you should consult with the team and be prepared to publicly document this exception.

### Public domain

[By law](http://www.law.cornell.edu/uscode/text/17/105), works of the United States government are not copyrightable in the US, and so are public domain. But by default, US government works **are** copyrightable internationally, and so NPMap intentionally waives this copyright abroad using [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

There are potentially other cases where copyright is involved: where contractors produce the work, or where work was otherwise originally performed not in the capacity of a US government employee.

To the extent NPMap has the rights to do so, NPMap will normalize the copyright status of its work product under CC0.

### Contributing back to outside projects

NPMap staff are encouraged to contribute back any modifications or improvements they make to open source software projects outside NPMap -- whether government or non-government -- in the course of their work. When NPMap staff begin modifications to outside work, they should plan with eventual upstream contribution in mind.

In terms of licensing: as works of the government, employee contributions are public domain in the United States, regardless of the outside project's contribution agreement. This does not change the overall license status of the outside project.

As [the Free Software Foundation says](https://www.gnu.org/licenses/gpl-faq.html#GPLUSGovAdd) about government-contributed improvements to GPL software:

> Yes. If the improvements are written by US government employees in the course of their employment, then the improvements are in the public domain. However, the improved version, as a whole, is still covered by the GNU GPL. There is no problem in this situation.

#### How to license NPMap repos

When you create a repo, add a [LICENSE.md](LICENSE.md) and [CONTRIBUTING.md](CONTRIBUTING.md) file, and add a [paragraph to the end of your README](README.md#public-domain).

The preceding links are to our standard boilerplate for each of those, so you can just copy and paste them. In some cases, you may need to customize them for your use -- for example, if you've forked a project that originated from outside the government.

You may wish to add the following to your `.bashrc` or `.zshrc`:

```bash
alias insert-license="curl -sO https://raw.githubusercontent.com/nationalparkservice/npmap-open-source-policy/master/LICENSE.md"
alias insert-contrib="curl -sO https://raw.githubusercontent.com/nationalparkservice/npmap-open-source-policy/master/CONTRIBUTING.md"
alias npmap-init="insert-license && insert-contrib && echo 'Licensed.'"
```

You can then initialize a new NPMap repository's license information with:

```bash
npmap-init
```

It's also recommended to copy and paste [this paragraph for the end of your README](https://github.com/nationalparkservice/npmap-open-source-policy/blob/master/README.md#public-domain) that sums up what's going on.

### Accepting contributions from the public

Any NPMap project can (and should!) accept open source contributions from the public.

Projects can **encourage public contributions** by:

* Creating open issues where public help would be especially welcome.
* Labeling those issues with `help-wanted` so people can scan issues quickly and [services](http://www.codeforamerica.org/geeks/civicissues) can aggregate volunteer opportunities.
* Asking for it, in the README and in other public writing about the project.
* Providing solid documentation for any project setup process.
* Being super nice when communicating with volunteers.

As [described above](#public-domain), NPMap projects are dedicated to the international public domain wherever possible. In this situation, contributors must agree to release their contributions into the international public domain. Projects can inform contributors of this agreement by copying the [`CONTRIBUTING.md`](CONTRIBUTING.md) file from this repo into new project repos, and copying the ["Public domain" section of this repo's README](README.md#public-domain) into the new project's README.

When an NPMap project has a non-standard license status (e.g. it's a fork of a previously licensed project, or is a module/plugin for a GPL project), then that project needs to figure out an appropriate contributing agreement.

### Working in public

NPMap believes in working in public. It creates a healthier working environment, a more collaborative process, and just better software.

All NPMap team members are expected to make new source code repositories public from the time of creation.

### Delays and exceptions

Our policy lists [3 classes of exceptions](https://github.com/nationalparkservice/npmap-open-source-policy/blob/master/policy.md#exceptions) for which we will not release source code:

1. We don't have the rights to release the code.
2. The code's public release is restricted by a specific law or regulation (for example, arms control).
3. Some other "compelling interest" that is "rare [and] documented publicly", listed below.

There are a couple of categories of "compelling interests" where we may _temporarily_ delay open sourcing our work:

* **Before the ink is dry**
* **Brief experimentation**
