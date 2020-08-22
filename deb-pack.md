# Building deb package

## Build dependencies

```
sudo apt-get --no-install-recommends install \
 debhelper dh-python devscripts
```

## Building package
To build binary package run following command in xubuntu-default-settings directory.
Non-signed binary package will be created in *parent directory*.

```shell
debuild -us -uc -b
```

## Installing package

```shell
sudo dpkg -i xubuntu-default-settings_20.10.0-sg.deb
```

Now you can safely remove fonts-noto-hinted package from the system