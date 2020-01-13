# ampache-docker

Docker container for Ampache, a web based audio/video streaming application and file manager allowing you to access your music & videos from anywhere, using almost any internet enabled device.

![travis status](https://travis-ci.org/arielelkin/ampache-docker.svg?branch=master)

## Usage

To run official builds from docker hub you can run these commands:

To run the current Ampache master (stable) branch
```bash
docker run --name=ampache -d -v /path/to/your/music:/media:ro -p 80:80 ampache/ampache
```

To run the current Ampache develop branch
```bash
docker run --name=ampache -d -v /path/to/your/music:/media:ro -p 80:80 ampache/ampache:develop
```

## Running on ARM

The automated builds for the official repo are now built for linux/amd64, linux/arm/v7 and linux/arm64.

## Installation
- MySQL Administrative Username: root    # leave alone
- MySQL Administrative Password: (blank) # leave alone
- Check "Create Database User"
- Ampache Database Username: ampache
- Ampache Database User Password: ampache # or whatever you want, but remember it on the next page
- next page fill out MySQL Username / Password
- Click the "Write" buttons from BOTTOM to TOP
- Do this because it is the last one that needs the username and password and they get blanked out on every click

## Thanks to
- @ericfrederich for his original work
- @velocity303 and @goldy for the other ampache-docker inspiration

## Current Release

4.1.0
