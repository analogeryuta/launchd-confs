launchd-confs
==========================

Launchd Configurations (OS X only).
---------------------------

## Howto Use

change paramaters for your environments:

```diff
- <string>/Users/freddie/.rbenv/shims/atig</string>
+ <string>/Users/john/.rbenv/shims/atig</string>
```

copy plist to your local machine:

```sh
$ cp atig.plist ~/Library/LaunchAgents/
```

load plist to launchd daemon:

```sh
$ sudo launchctl load ~/Library/LaunchAgents/atig.plist
```
