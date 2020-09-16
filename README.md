Heroku buildpack: Taglib
=======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for using [taglib](http://taglib.github.io/) in your project.  

NOTE : because the debian lib was built using shared libs we had to include `libicu63` too

Usage
-----

Simply add this buildpack in your heroku dashboard **before** your Ruby build pack.

You can verify installing taglib by following command.

    $ heroku run "taglib-config"

Updating taglib
---------------

The included binaries are from the following debian packages, if you want to updated to a new version you should download the updated packages and update the `.tar.gz` archive in this repo.

- `libtag1-dev_1.11.1+dfsg.1-0.3+deb10u1_amd64`
- `libtag1v5-vanilla_1.11.1+dfsg.1-0.3+deb10u1_amd64`
- `libtagc0_1.11.1+dfsg.1-0.3+deb10u1_amd64`
- `libtagc0-dev_1.11.1+dfsg.1-0.3+deb10u1_amd64`
- `libicu63_63.1-6+deb10u1_amd64`
