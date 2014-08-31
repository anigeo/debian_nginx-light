# nginx-light on Debian Wheezy Backports

Automatic docker image build with nginx-light wheezy-backports packages.  Visit <https://packages.debian.org/wheezy-backports/nginx-light> for package detail.

## Usage
```
docker run -d -v <path to sites config>:/etc/nginx/sites-enabled:ro -p 80:80 anigeo/debian_nginx-light:latest
```

## Note
Both access_log and error_log are disabled by default, use volume bind mount (-v) custom config if you would like to enable.
