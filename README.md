![Banner](banner.png)

# monitor-securityevents
Monitors the Windows Security Event Log for specific events, allowing filtering by Event ID, source, and user. Uses the `pywin32` library (the win32evtlog, win32evtlogutil, and win32security modules, installed as the single pywin32 package in requirements.txt) for log access and filtering. In persist mode only events newer than the highest record number already seen are reported, so events are not reprinted on every cycle. A non positive `--interval` exits with code 1 at startup. - Focused on System monitoring and alerts

## Install
`git clone https://github.com/ShadowGuardAI/monitor-securityevents`

## Usage
`./monitor-securityevents [params]`

## Parameters
- `-h`: Show help message and exit
- `--event-id`: Filter events by Event ID.
- `--source`: No description provided
- `--user`: No description provided
- `--interval`: No description provided
- `--persist`: Keep running and monitoring the event log indefinitely.
- `--debug`: Enable debug logging.

## License
Copyright (c) ShadowGuardAI
