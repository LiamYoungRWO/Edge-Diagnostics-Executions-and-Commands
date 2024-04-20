# System Clock Commands and Functions

## Using Date/Time Approach: Proper Order of Operations

### Beggining with seerver clock system diagnosis


#### We begin by checking the current time

```bash
date
```

#### Then Check the status of the Network Time Protocol (NTP) service to ensure it's syncing correctly:

```bash
timedatectl status
```

#### In the event NTP is not enabled, we can manually force a sync with NTP servers:

```bash
sudo systemctl restart systemd-timesyncd
```
