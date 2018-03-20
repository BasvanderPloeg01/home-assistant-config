# Notifications

Useful during development of automations, I later keep using them for simple warnings like when the dehumidifier is likely full in [`/automations/check_humidity_high.yaml`](../automations/check_humidity_high.yaml)  or if a door has been left open for too long in [`/automations/check_doors.yaml`](../automations/check_doors.yaml).

## Organization

### [`👪 ./groups.yaml`](groups.yaml)

Notifications services are organized into higher-level [notification groups](https://home-assistant.io/components/notify.group/), to avoid peppering hard-coded services throughout automations.


### [`📢 ./lannouncer.yaml`](lannouncer.yaml)

For audio alerts and text-to-speech messages sent to the [LANnouncer](http://www.keybounce.com/lannouncer/) Android app running on the kiosk.


### [`💬 ./pushover.yaml`](pushover.yaml)

Notification service for cellphones and tablets. I was already using [Pushover](https://pushover.net) for other purposes, so might as well continue.
