# sitespeed.io

This Docker get you [sitespeed.io](http://www.sitespeed.io) with Firefox & Xvfb installed.

## Usage

The ```--rm -v "$(pwd)":/sitespeed.io``` will make the result HTML stored on your host.

### Analyze a site and fetch timings using Firefox
```
docker run --privileged --rm -v "$(pwd)":/sitespeed.io sitespeedio/sitespeed.io-firefox sitespeed.io -u http://www.sitespeed.io -b firefox --seleniumServer http://127.0.0.1:4444/wd/hub
```

## Configuration
sitespeed.io is highly configurable, check the [documentation](http://www.sitespeed.io/documentation).
