# ybp - Execute command in hybris/bin/platform

When working with SAP Commerce, you have to execute most of the interesting
commands like `ant` or `hybrisserver.sh` in the `hybris/bin/platform` directory.

This little wrapper takes care of the navigation, regardless in what folder of the 
project you are, and also sources `setantenv.sh`, if necessary

## Installation

1. Clone or download this repo
1. `chmod u+x ybp`
1. put `ybp` somehwere on your `PATH`
1. Never type `cd ../../../hybris/bin/platform` or `source setantenv.sh` again

## Examples

```
ybp ant clean all
# run ant clean all for the whole platform

ybp ./hybrisserver.sh debug
# start server
```

## Hint

- For maximum ~~laziness~~ developer efficiency, define an alias for `ybp ant`, e.g
  `alias ya='ybp ant'`