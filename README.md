![dotProject Logo](style/nord/images/favicons/android-chrome-96x96.png)
# dotProject
**dotProject** is an open source project management system written in PHP.

It originally started in 2001 by dotMarketing on SourceForge and has
been under the watchful eye of the current dotProject team since around December 2002.

## Disclaimer

This is [Gwyneth Llewelyn](https://github.com/GwynethLlewelyn)'s fork, to provide PHP 8.0+ support and a few extra goodies. While I maintain a separate list of issues, these are strictly related to this fork, and not to the overall dotProject code, which is officially maintained by the community.

The only reason for this fork to exist is because many need full PHP 8.0+ support (now that even 7.4 reached EOL), including, of course, myself. This fork is solely kept as an ongoing PR to the main development branch of dotProject, where hopefully it will be integrated at some point in time.

## Installing/Upgrading

**NOTE** The `devel` branch is where all the development happens.  If you want the latest and greatest with all relevent bug fixes between releases, then download from https://github.com/dotproject/dotProject/archive/devel.zip

`master` tracks the current release.

**The Quick Way**: Point your browser to the `install` directory.

## Support

Support forums are at http://forums.dotproject.net/index.php

Bug reports and other issues can be lodged on GitHub at https://github.com/dotproject/dotProject/issues

IRC channel is irc://irc.freenode.net/dotproject on `#dotproject` on `irc.freenode.net`

## License

As of version 2.0, dotProject is released under [GPL](LICENSE.md).
1.0.2 and previous versions were released under BSD license.
Parts of dotProject include libraries from other projects which are used and re-released under their original licence.

## Docker composer support

The latest devel branch now includes a simple `docker-compose.yml` file and support files.  These will allow you to run dotProject by running:

`docker-compose up`

This will set up an nginx container, a phpfpm container and a mariadb container and point the web server to the base directory of dotProject.  All you need to do after that is point your browser to http://localhost/

`docker-compose down` will retain any data you have created.  If you want to start again from a clean slate, use `docker-compose down -v` to remove the database volume.

