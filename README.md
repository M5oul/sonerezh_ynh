# Sonerezh package for YunoHost

[![Integration level](https://dash.yunohost.org/integration/sonerezh.svg)](https://dash.yunohost.org/appci/app/sonerezh) ![](https://ci-apps.yunohost.org/ci/badges/sonerezh.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/sonerezh.maintain.svg)

* [Sonerezh website](https://www.sonerezh.bzh/)
* [YunoHost website](https://yunohost.org/)

![Sonerezh screenshots](screenshots.png)


## Postinstallation
Currently, you will have to do manually postinstallation.
There is [an issue](https://github.com/YunoHost-Apps/sonerezh_ynh/issues/1) to solve that issue. But I wasn't able to solved it.

You will have to go to `/sonerezh/install/` and put this parameters:

- Retrieve database password:
```bash
sudo cat /etc/yunohost/apps/sonerezh/settings.yml | grep mysql
```
- Put your email and password to create an account.

![Postinstall](postinstall.png)

## Music
Actually, Sonerezh do not provide a web interface to upload music.
You have to store your music in `/home/yunohost.app/sonerezh`.
Sonerezh will update your music.
