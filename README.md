# Blocklists

Annoyances blocklists for Pi-hole/uMatrix/AdGuard Home and Adblock/uBlock. 

These blocklists will break some things you might want to keep operational (especially when used with a DNS sinkhole), for example push notifications, automatic updates for various devices, etc.

## Pi-hole

Use `pihole -w $(cat whitelist.txt)` to add entries to whitelist. 

Use `pihole -b $(cat dns_sinkhole.txt)` to add entries to blacklist. 

Use `pihole --regex $(cat wildcards.txt)` to add entries to regex blacklist.
