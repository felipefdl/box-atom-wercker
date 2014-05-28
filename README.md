## Wercker box to Atom.io build

Box with all tools to build package for atom.io

## Code Status
[![wercker status](https://app.wercker.com/status/2a72222f9c13b9e77eb2a11d1f79e2e7/m "wercker status")](https://app.wercker.com/project/bykey/2a72222f9c13b9e77eb2a11d1f79e2e7)

## Usage
Add this step before any step
``` yml
- script:
    name: Enable virtual display
    code: |-
        export DISPLAY=:99.0
        start-stop-daemon --start --quiet --pidfile /tmp/xvfb_99.pid --make-pidfile --background --exec /usr/bin/Xvfb -- :99 -screen 0 1024x768x24 -ac +extension GLX +render -noreset
        sleep 3
```

## Example:
Atom.io Plugin - [Wercker Status](https://github.com/felipefdl/wercker-status)

## License

Wercker box to Atom.io is released under the [MIT License](https://github.com/felipefdl/box-atom-wercker/blob/master/LICENSE.md).

[![Gittip](http://img.shields.io/gittip/felipefdl.svg)](https://www.gittip.com/felipefdl)
