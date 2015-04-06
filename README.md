# munin-plugin-wget

This plugin will download content from specified URL, and report the time it takes to download as well as the size of the output.

## Installation

Git clone somewhere.. then create a symlink in /etc/munin/plugins
```
cd /etc/munin/plugins
sudo ln -s /home/hayashis/git/munin-plugin-wget/wget wget
```
(adjust the location)

You then need to reload your munin-node
```
sudo /etc/init.d/munin-node reload
```

## Configuration

Add your configuration in /etc/munin/plugin-conf.d/wget and specify parameters that you want to monitor

```
[wget]
env.url "http://google.com"
```

