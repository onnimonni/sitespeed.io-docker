# sitespeed.io

This Docker get you [sitespeed.io](http://www.sitespeed.io) with Chrome and Xvfb installed.

## Usage

The ```--rm -v "$(pwd)":/sitespeed.io``` will make the result HTML stored on your host.

### Analyze a site and fetch timings using Chrome
```
docker run --privileged --rm -v "$(pwd)":/sitespeed.io sitespeedio/sitespeed.io-chrome sitespeed.io -u http://www.sitespeed.io -b chrome --seleniumServer http://127.0.0.1:4444/wd/hub
```

## Configuration
sitespeed.io is highly configurable, check the [documentation](http://www.sitespeed.io/documentation).
