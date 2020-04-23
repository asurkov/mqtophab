# mqtophab

Sends all applied (hg qapp) MQ patches to Phabricator. It is a bash wrapper around [moz-phab](https://moz-conduit.readthedocs.io/en/latest/phabricator-user.html#submitting-patches) tool.

## How to use

``bash mqtophab.sh``

## Notes

Make sure to disable `histedit` extension since it doesn't seem working well with mercurial queues: when you do `qdel`/`qimp` bundle, it adds multiple commits of the same revision. In order to disable it open `~/.hgrc` and change `histedit = ` to `#histedit = `.
