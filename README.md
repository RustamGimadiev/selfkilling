## About
Yet another time bomb for automatic cleaning up Helm releases

### Usage
This chart could be added as requirement sub-chart to your own umbrella-chart. You could configure a working of this chart by next options:

| Option | Description | Default value |
| ------ | ----------- | ------------- |
| `ttl.enabled`| Set `false` to disabling selfkilling | `True`|
| `ttl.minutes`| Number of minutes before selfkilling | `1`   |

### How it works
Based on https://blog.ropnop.com/attacking-default-installs-of-helm-on-kubernetes was create yet another time bomb container, it launched as a CronJob.
