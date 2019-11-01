This is the older version of smbclient that showed the version of samba when getting information about Windows clients. It also includes [enum4linux](https://github.com/portcullislabs/enum4linux).

# Install
Only one of these will work. Try the newer version first, if it doesn't work try the older one.

## Newer versions of Kali
`apt-get install docker-ce`

## Older versions of Kali
`apt-get install docker-io`

# Usage
You can use the smbclient and enum4linux like normal after the docker run command setup.

```docker run --rm tanglisha/enum4linux-old-smbclient smbclient -L -I [IP]```

or

```docker run --rm tanglisha/enum4linux-old-smbclient enum4linux /[SHARENAME]```

It'll take a bit to download the first time you run it.

There are also a couple of bash files in the `bin` directory that you can run if you don't feel like typing all of that out. `./enum4linux-old` and `./smbclient-old`. Add the bin to your PATH if you want to be REALLY lazy.
