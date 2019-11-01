This is the older version of smbclient that showed the version of samba when getting information about Windows clients. It also includes enum4linux.

# Install
To use on Kali, first install docker. On newer versions of Kali, you'll want to install `docker-ce`, on older versions you'll want `docker.io`.

# Usage
You can use the smbclient and enum4linux like normal after the docker run command setup.

```docker run --rm tanglisha/enum4linux-old-smbclient smbclient -L -I [IP]```
or
```docker run --rm tanglisha/enum4linux-old-smbclient enum4linux /[SHARENAME]```

It'll take a bit to download the first time you run it.
