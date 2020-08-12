# Blocklists

Annoyances blocklists for Pi-hole/uMatrix/AdGuard Home and Adblock/uBlock. 

These blocklists will break some things you might want to keep operational (especially when used with a DNS sinkhole), for example push notifications, automatic updates for various devices, etc.

## Pi-hole

* Use `pihole -w $(cat whitelist.txt)` to add entries to whitelist. 

* Use `pihole -b $(cat dns_sinkhole.txt)` to add entries to blacklist. Alternatively, add a list at `/admin/groups-adlists.php`

* Use `pihole --regex $(cat wildcards.txt)` to add entries to regex blacklist.

## uMatrix

If a domain is present in an uMatrix blocklist, all it's subdomains are also blocked. Blocking `example.com` will also block `subdomain.example.com`.
