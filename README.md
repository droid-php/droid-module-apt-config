# Droid Module: droid/apt-config

Configure Apt. This module will configure Apt to permit the packaged cron jobs
to trigger automatic updates of the package lists. This configuration may be
overridden to set whatever options you wish.

For more information on Droid, please see [droidphp.com](http://droidphp.com).

The steps involved are:-

1. Create `/etc/apt/apt.conf` where it does not exist.
2. Write configuration values to `/etc/apt/apt.conf`.


## Assumptions

1. The platform is Debian-based.


## Limitations

None.


## Information required by the module

None.


## Optional information

1. Configuration values, as follows:-

        variables:
          apt_config:
            - [<string>, <string>] # e.g. ["APT::Periodic::RandomSleep", "0"]
