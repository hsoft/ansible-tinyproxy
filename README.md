# ansible-tinyproxy

*Provisions a simple [tinyproxy][tinyproxy] server.*

Mostly for quick-and-dirty personal proxy to get around region-based content blocking. Spawn a VM
in the same country where you want to access your content and add your IP to `tinyproxy_allows`.

## Requirements

* Ansible 2.0+
* Debian jessie target

## Example

```
- role: tinyproxy
  tinyproxy_allows:
    - 1.2.3.4
```

[tinyproxy]: https://tinyproxy.github.io/
