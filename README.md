# ansible-resolvconf
* * *

## Description

Set /etc/resolv.conf file.

Warning: this role ensures that /etc/resolv.conf is not a symbolik link. In the case it is a symbolik link it first deletes it before writing the new resolv.conf file.

## Variables

- _dns_nameservers_: list with name servers.
- _dns_search_: string.

_dns_nameservers_ defaults to 8.8.8.8 and 8.8.4.4 if no values are provided.
