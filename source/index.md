
NEO-AS: AS4242421123
========================================

I operate `AS4242421123` on [dn42](https://dn42.info/Home), an open & collaborative networking sandbox.

I also operate a looking glass at [dn42.ccp.ovh](https://dn42.ccp.ovh) and [n.dn42](http://n.dn42)

Network Map
----------------------------------------
![network map](https://maps.googleapis.com/maps/api/staticmap?center=&zoom=1&scale=false&size=640x200&maptype=roadmap&key=AIzaSyCSioCrhT9ObSnQqgqWMRodvjSPjhBrOss&format=png&visual_refresh=true&markers=icon:https://rawcdn.githack.com/Novik/ruTorrent/a4a68f87d4a44800325a22a1acf484239cd17d0a/plugins/geoip/flags/us.gif%7Cshadow:true%7CLAX&markers=icon:https://rawcdn.githack.com/Novik/ruTorrent/a4a68f87d4a44800325a22a1acf484239cd17d0a/plugins/geoip/flags/hk.gif%7Cshadow:true%7CHKG&markers=icon:https://rawcdn.githack.com/Novik/ruTorrent/a4a68f87d4a44800325a22a1acf484239cd17d0a/plugins/geoip/flags/nl.gif%7Cshadow:true%7CAmsterdam)


Peering Policy
----------------------------------------
New peers are always welcome - free to reach out via IRC (mayli#dn42@hackint) or [NEO-DN42](https://git.dn42.dev/dn42/registry/src/branch/master/data/person/NEO-DN42).
Currently my PoPs only support **WireGuard**.

For consistency, I prefer _multiprotocol BGP_ sessions over IPv6. For WireGuard + BIRD users, I recommend using link-local IPv6 addresses. 
If you have multiple nodes, especially across multiple continents, I also recommend setting up multiple links to improve redundancy and encourage the most direct routing.

Inactive peers may be removed after a certain amount of time.


Node information
----------------------------------------

All following nodes are opening for peering over wireguard.

| Region | Hostname    | AS  | WireGuard Port | WireGuard Pubkey | Tunneled IPv4 | Tunneled IPv6 |
| ---    | ----        | --- | ---            | ---              | --            | --            |
| LAX    | lax.ccp.ovh | `4242421123` | \* | `Z6OKJSR1sxMBgUd1uXEe/UxoBsOvRgbTnexy7z/ryUI=` | `172.20.47.1` | `fe80::1123` |
| AMS    | ams.ccp.ovh | `4242421123` | \* | `e5X1ZlZUOVtTFeWi+d6cUqqNaXB0F2UHwbquAKU4z3I=` | `172.20.47.2` | `fe80::1123` |
| HKG    | hkg.ccp.ovh | `4242421123` | \* | `bLysMVqew2hlvJVS17hp+qaURzZuLERLgfSbvK/mgUU=` | `172.20.47.3` | `fe80::1123` |

\*: My local port will be *last 5 digits of your ASN*

Manual peering
----------------------------------------
To establish a peer with me, the following information is required:

        Your ASN (DN42)
        The node you would like to peer
        Your tunnel endpoint
        Your wireguard public key
        Your tunnel link addresses: Tunneled IPv6, Tunneled IPv4(optional)
        Options features: MPBGP(default on), extended next hop(default on)

Automated peering
----------------------------------------
Coming Soon(tm)
