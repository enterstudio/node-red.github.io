---
layout: docs
toc: getting-started-toc.html
title: Installation
---

### Install node.js

We recommend the use of node.js **LTS 6.x**. Node-RED no longer supports node.js 0.10.x or 0.12.x.

You can get the latest Long Term Support (LTS) version of Node <code>6.x</code> from the nodejs [download site](https://nodejs.org/en/download/).

It is often easiest to use a [packaged version](https://nodejs.org/en/download/package-manager/)
specifically for your operating system.

We also have specific instructions available for certain hardware platforms and operating systems:

 - [Raspberry Pi](../hardware/raspberrypi)
 - [BeagleBone Black](../hardware/beagleboneblack)
 - [Windows](../platforms/windows)

Other download options are available [here](https://nodejs.org/dist/latest-v6.x/).

### Install Node-RED

The easiest way to install Node-RED is to use node's
package manager, npm. Installing it as a global module adds the command `node-red`
to your system path:

    sudo npm install -g --unsafe-perm node-red

<div class="doc-callout">
<em>Note</em>: <code>sudo</code> is only required during the install when running on Linux or OS X. If
running on Windows, see the <a href="../platforms/windows">Windows Install instructions</a>.
</div>

#### Next

Once installed, you are ready to [run Node-RED](running).

----

### Alternative install methods

#### Download a release

You can download the latest release from [here](https://github.com/node-red/node-red/releases/latest).
The zip contains a top-level folder called `node-red-X.Y.Z` where `X.Y.Z` is the
version number. Once extracted, from within that top-level folder, run the
following command:

    npm install --production

#### For Development - from GitHub

Running the code from GitHub is only intended for users who are happy to be using
development code, or for developers wanting to contribute to the code.

You can clone the source repository directly from GitHub:

    git clone https://github.com/node-red/node-red.git

Once cloned, the core pre-requisite modules must be installed :

    cd node-red
    npm install

<div class="doc-callout">
<em>Note</em>: when running from a clone of the git repository, it is necessary
to install all dependencies, not just the production level ones. This is why the
 <code>--production</code> option should not be used.
</div>

You will also need to install `grunt-cli` in order to build the application before
you can use it. This must be done globally.

    sudo npm install -g grunt-cli

You can then build and run the application

    grunt build
    node red

### Next steps

Once installed, you are ready to [run Node-RED](running).
