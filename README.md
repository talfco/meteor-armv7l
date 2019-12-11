# Meteor enablement for running on an armv7lv architecture

This is a clone of Meteor V1.5.2.2 and contains changes in the scripts in order to build and run Meteor on Linux ARM architecture of the 7th version, named `armv7l`. This CPU architecture can be found for example in the [Odroid-HC2](https://www.hardkernel.com/shop/odroid-hc2-home-cloud-two/)

You can search for `*.old` files in order to understand which files got changed.

## Installation Instructions

* login to your armv7l device
* clone this repository
* change in the cloned directory
* execute `./scripts/generate-dev-bundle.sh`, which builds the `dev-bundle`
* include the meteor directory in you path and switch over to your meteor project and start the app

Thanks goes to
* https://meteor-universal.tumblr.com/
* https://github.com/4commerce-technologies-AG/meteor
* https://github.com/4commerce-technologies-AG/meteor/issues/67
" https://github.com/Gatux/meteor

Meteor-Release which was used as a base: 1.5.2.2

* `git clone --single-branch --branch "release-1.5.2.2" https://github.com/meteor/meteor.git`

The script files are minimal, so it's quite ease to modify them to run another older version of Meteor on a ARM based architecture.

Allowed me to shift a cloud based Meteor App instance to a self-hosted, cost and power-efficient Odroid-HC2 machine. 


# <a href='https://www.meteor.com'><img src='https://user-images.githubusercontent.com/841294/26841702-0902bbee-4af3-11e7-9805-0618da66a246.png' height='60' alt='Meteor'></a>

[![TravisCI Status](https://travis-ci.org/meteor/meteor.svg?branch=devel)](https://travis-ci.org/meteor/meteor)
[![CircleCI Status](https://circleci.com/gh/meteor/meteor/tree/devel.svg?style=shield&circle-token=c2d3c041506bd493ef3795ffa4448684cfce97b8)](https://circleci.com/gh/meteor/meteor/tree/devel)

Meteor is an ultra-simple environment for building modern web
applications.

With Meteor you write apps:

* in modern JavaScript
* that send data over the wire, rather than HTML
* using your choice of popular open-source libraries

Try a getting started tutorial:
 * [React](https://www.meteor.com/tutorials/react/creating-an-app)
 * [Blaze](https://www.meteor.com/tutorials/blaze/creating-an-app)
 * [Angular](https://www.meteor.com/tutorials/angular/creating-an-app)

Next, read the [guide](https://guide.meteor.com) and the [documentation](https://docs.meteor.com/).

## Quick Start

On Windows, the installer can be found at https://www.meteor.com/install.

On Linux/macOS, use this line:

```bash
curl https://install.meteor.com/ | sh
```

Create a project:

```bash
meteor create try-meteor
```

Run it:

```bash
cd try-meteor
meteor
```

## Developer Resources

Building an application with Meteor?

* Announcement list: sign up at http://www.meteor.com/
* Having problems? Ask for help at: http://stackoverflow.com/questions/tagged/meteor
* Discussion forums: https://forums.meteor.com/

Interested in helping or contributing to Meteor?  These resources will help:

* [Core development guide](Development.md)
* [Contribution guidelines](Contributing.md)
* [Feature requests](https://github.com/meteor/meteor-feature-requests/)
* [Issue tracker](https://github.com/meteor/meteor/issues)

We are hiring!  Visit [meteor.io/jobs](https://www.meteor.io/jobs/) to
learn more about working full-time on the Meteor project.

## Uninstalling Meteor

Aside from a short launcher shell script, Meteor installs itself inside your
home directory. To uninstall Meteor, run:

```bash
rm -rf ~/.meteor/
sudo rm /usr/local/bin/meteor
```

On Windows, just run the uninstaller from your Control Panel.
