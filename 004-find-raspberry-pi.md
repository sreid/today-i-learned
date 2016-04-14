# Find a Raspberry Pi on a Network
Looking for the IP address of a headless Raspberry Pi, so you can SSH to it? Try:

```
arp -a | grep b8:27:eb | grep -Eo '[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}'
```

Note: This method isn't foolproof. If nmap is available, you may be able to scan for it (see link below). But it seems to work 90% of the time.

Hat Tip: http://serialized.net/2013/04/headless_rpi/
