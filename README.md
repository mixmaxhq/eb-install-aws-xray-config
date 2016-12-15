# eb-install-aws-xray-config

This module installs an `.ebextensions` config file that will install
and start the AWS XRay daemon.

## Installation

1. `npm install eb-install-aws-xray-config --save`
2. Commit the `.ebextensions` file it creates.
3. Deploy.

## Modifying the `.ebextensions` file

This module will overwrite the file if/when it is updated.

Pull requests are welcome if you have some generally-useful modifications to
suggest.

If you'd like to make modifications specific to your use case, you should uninstall
this module after installing the `.ebextensions` file. Uninstallation won't take
the file with it.

## Based off of

This module is based off of [eb-authenticate-npm](https://github.com/mixmaxhq/eb-authenticate-npm).

## Extra resources:

If you're new to using AWS XRay with Elastic Beanstalk, you'll want to checkout
[the docs](https://docs.aws.amazon.com//xray/latest/devguide/xray-daemon-beanstalk.html).
You'll also want to ensure you're EC2 instances have the
[correct permissions](https://docs.aws.amazon.com/xray/latest/devguide/xray-daemon.html#xray-daemon-permissions).
