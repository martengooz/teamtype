<!--
SPDX-FileCopyrightText: 2024 blinry <mail@blinry.org>
SPDX-FileCopyrightText: 2024 zormit <nt4u@kpvn.de>

SPDX-License-Identifier: CC-BY-SA-4.0
-->

# Configuration

You can put the following options into a configuration file at `.teamtype/config`:

```ini
username = <string>
peer = <secret_address>
emit_join_code = <true/false>
emit_secret_address = <true/false>
magic_wormhole_relay = <magic_wormhole_mailbox_relay_url>
iroh_relay = <iroh_relay_server_url>
```

After a successful `teamtype join`, the peer's secret address is automatically stored in your `.teamtype/config`.
In the future, you can then use `teamtype join` without a join code to reconnect to the same peer.

## Custom Iroh relay server

The `iroh_relay` setting allows you to use a custom Iroh relay server instead of the default n0 relays. This is useful if you want to run your own relay infrastructure or use a private relay server.

You can also use the `--iroh-relay` flag:

```bash
teamtype share --iroh-relay https://my-relay.example.com:port
```
