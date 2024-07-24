## Overview
pndeploy is a tool to deploy Pane System Images and create custom installers for mass deployments on a fleet of devices.

## Arguments
`-I`: short for _Install_, takes a path to a Pane System Image file. (.iso, .psi)
`-D`: short for _Disk_, specifies the disk to deploy the image on. If only one disk is installed, this may be omitted.
`-R`: short for _RAID_, configures the image to work on a RAID disk setup. This takes `mirror | parity | striped` as arguments.
`-E or --edition-`: specify with edition of PaneOS to install. If not specified, it will always deploy PaneOS Professional.
