# mqtophab

Sends all applied (hg qapp) MQ patches to Phabricator. It is a bash wrapper around [phabsend](https://bitbucket.org/kmaglione/hgext/src/default/phabricator.py) extension.

# How to install
* download the [phabricator.py file](https://bitbucket.org/kmaglione/hgext/src/default/phabricator.py), put it somewhere and then in your `~/.hgrc` add
```phabsend = /path-to/phabricator.py``` in the [extensions] section
* intialzie [phabricator] and [auth] sections, see [mailing list post](https://groups.google.com/d/msg/mozilla.dev.platform/o9f2S0vO47k/IJZJSEBcCAAJ) for details.
