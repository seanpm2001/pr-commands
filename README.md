Pull Request Commands for Salt Open
===================================

The repository contains the code used to run tests from commenting on a pull
request.

Usage
=====

```text
re-run [full] all|jenkins-job-name
```

Running `full` means that all tests are run instead of just things that changed in the PR.

The job name is found in the jenkins url, such as pr-ubuntu2004-py3-pytest in https://jenkins.saltproject.io/job/pr-ubuntu2004-py3-pytest/job/PR-59710/

If `all` is used as the last arg, all jobs are re-run, otherwise anything matching a substring of the job name, or the
whole job name will be run.

Examples
========

- re-run full all
- re-run all
- re-run centos
- re-run centos7
- re-run full pr-photon3-py3-pytest
