# leaktk-github-monitor

A process that monitors GitHub for certain events

## Requirements

* Do a long running check that goes through the repos it monitors and checks for any changes in the last 30 days
* Support integrating with the github event API and do optimized poling based on the rate limit
* Support both using an access token or using GitHub app credentials for higher rate limits through enterprise accounts
* Support hourly pulling of gharchive
* Support chosing the source of the events above via a config file
* Output leaktk-scanner requests
* Support a mapping of repos to monitor to identities
