# tt-desk

A one-file forwarding page. It holds no data and no key: it reads `target.json` (the current address of a
privately served dashboard) and sends the visitor there, passing along the `?k=` part of their link.

`target.json` is rewritten and pushed by `ops/share_tunnel.py` in the dashboard's own repository whenever
the address changes. Don't edit it by hand.
