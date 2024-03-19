# AdGuardHome
Files I use for AdGuard Home on my home network and also on my laptop (when not on my home network).
AdGuard Home runs in a Docker container on Raspberry Pi (on my home network).
And in a Docker container locally on my Mac (when I'm not at home).
While AdGuard Home is also used for its DHCP server on home network, I use AdGuard Home only for DNS lookups when I'm away from home (at a library, café, airport, hotel, etc). I've found AdGuard Home to be quite effective.

# for container on local machine
docker compose -f adguardhome_local.yaml --env-file .local_env  up -d

# for container on home network
docker compose -f adguardhome_network.yaml up -d
