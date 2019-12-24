# PULL_REQUEST_TEMPLATE.md

```md
<!--
Please make sure you've read and understood our contributing guidelines;
https://opensource.bloom.sh/contributing

** Make sure all your commits include a signature generated with `git commit -s` **


If this is a bug fix, make sure your description includes "fixes #xxxx", or
"closes #xxxx"

Please provide the following information:
-->

**- What I did**

**- How I did it**

**- How to verify it**

**Which issue(s) this PR fixes**:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests or flakes`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #

**Special notes for your reviewer**:

**- Description for the changelog**
<!--
Write a short (one line) summary that describes the changes in this
pull request for inclusion in the changelog:
-->
```

# ISSUE_TEMPLATE

## bug-report.md

```md
---
name: Bug Report
about: Report a bug encountered while operating {PROJECT}
labels: kind/bug

---

<!-- Please use this template while reporting a bug and provide as much info as possible. Not doing so may result in your bug not being addressed in a timely manner. Thanks!-->


**What happened:**:

**What you expected to happen:**:

**Steps to reproduce the issue:**:

**Anything else we need to know?**:

**Environment:**:
- {PROJECT} version:
- OS:
- Others:
```

## enhancement.md

```md
---
name: Enhancement Request
about: Suggest an enhancement to the {PROJECT} project
labels: kind/feature

---
<!-- Please only use this template for submitting enhancement requests -->

**What would you like to be added**:

**Why is this needed**:
```


## support.md

```md
---
name: Support Request
about: Support request or question relating to {PROJECT}
labels: triage/support

---
```