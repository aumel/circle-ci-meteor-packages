circle-ci-meteor-packages
=========================

###Utilities for running Circle CI tests on Meteor Packages (tinytest).

Fork modified from arunoda/travis-ci-meteor-packages to work with Circle CI.

Add following file to your meteor package as `.circle.yml`

```
machine:
  node:
    version: 0.10.33
  pre:
    - curl -L https://git.io/vKvb4 | /bin/sh
test:
  override:
    - node /home/ubuntu/start_test.js
```
