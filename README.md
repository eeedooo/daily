# Daily

[![Build Status](https://travis-ci.org/pexcn/daily.svg?branch=master)](https://travis-ci.org/pexcn/daily)

This script can be automatically generate something what I needed every day.

## Usage

See [docs](docs).

- [`chnroute/chnroute.txt`](https://pexcn.me/daily/chnroute/chnroute.txt)
- [`adblock/adblock.conf`](https://pexcn.me/daily/adblock/adblock.conf)
- [`safelist/safelist.conf`](https://pexcn.me/daily/safelist/safelist.conf)
- [`pac/gfwlist.pac`](https://pexcn.me/daily/pac/gfwlist.pac)
- [`pac/whitelist.pac`](https://pexcn.me/daily/pac/whitelist.pac)
- [`shadowrocket/gfwlist.conf`](https://pexcn.me/daily/shadowrocket/gfwlist.conf)
- [`shadowrocket/whitelist.conf`](https://pexcn.me/daily/shadowrocket/whitelist.conf)
- More:
  - [`adlist`](https://github.com/pexcn/daily/tree/gh-pages/adlist)
  - [`gfwlist`](https://github.com/pexcn/daily/tree/gh-pages/gfwlist)
  - [`chinalist`](https://github.com/pexcn/daily/tree/gh-pages/chinalist)
  - [`alexa`](https://github.com/pexcn/daily/tree/gh-pages/alexa)

### OpenWRT

1. Save your needed [`scripts`](openwrt) into OpenWRT.
2. Add the following cron jobs.

```bash
# adblock
0 3 * * * <path/to/adblock_script>

# chnroute (chinadns)
1 3 * * * <path/to/chnroute_chinadns_script>

# chnroute (cleandns)
2 3 * * * <path/to/chnroute_cleandns_script>

# safelist
3 3 * * * <path/to/safelist_script>
```

## Credits

- [@shadowsocks/ChinaDNS](https://github.com/shadowsocks/ChinaDNS)
- [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)
- [@clowwindy/gfwlist2pac](https://github.com/clowwindy/gfwlist2pac)
- [@rssnsj/network-feeds](https://github.com/rssnsj/network-feeds)
- [@R0uter/gfw_domain_whitelist](https://github.com/R0uter/gfw_domain_whitelist)
- [@breakwa11/gfw_whitelist](https://github.com/breakwa11/gfw_whitelist)
- [@breakwa11/GFWList2PAC](https://github.com/breakwa11/GFWList2PAC)
- [@Leask/Flora_Pac](https://github.com/Leask/Flora_Pac)
- [aggregate](https://ftp.isc.org/isc/aggregate/)
- [cidrmerge](http://cidrmerge.sourceforge.net)

## License

```
Copyright (C) 2018-2019, pexcn <i@pexcn.me>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
```
