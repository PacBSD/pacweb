# Pacweb

This is the public facing website for PacBSD, build using
[Hugo](https://gohugo.io/) static site generator.

## Setup

To setup Hugo for development, follow [the installation
instructions](https://github.com/spf13/hugo#choose-how-to-install) on Github.

After cloning the repo copy _example-config.toml_ to _config.toml_.

## Running in development mode

Within the repo run the following in a terminal

    $ hugo serve

This will spin up a webserver on port 2015 (defined in _config.toml_), and build
the site watching for changes within the root directory of the repo.  When
changes are made `hugo` will rebuild the site and auto reload the site in the
browser(s).

## Building for production

To build the site for the production server run the following in a terminal

    $ hugo --config config-deploy.toml

This will build the static site, using the value of `baseurl` variable in the
_config-deploy.toml_ file.  The generated website is placed within the _public_
directory and can be copied to the production server.
