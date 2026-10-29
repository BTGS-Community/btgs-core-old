# Bitcoin Gold BTGS (BTGS Core)

Node and wallet software for the **existing BTGS chain**, maintained by the BTGS Community.

> The original developer left the project in 2026. This repository is the community-maintained version of the BTGS Core source (based on Bitcoin Core 30.2). A relaunch of BTGS on a new Dash-based chain is being prepared through community votes; until then, this is the software for the current chain.

## Chain details

| | |
| :--- | :--- |
| Algorithm | SHA-256 (proof of work) |
| Block time target | 10 minutes |
| Difficulty adjustment | every 1,008 blocks |
| P2P port | 18888 |
| RPC port | 18881 |
| Addresses | `G...` (legacy), `bcg1...` (SegWit) |

## Download

Ready-made wallets (Windows and Linux) with SHA256 checksums:
**https://github.com/BTGS-Community/btgs-wallet/releases**

Releases are built with **Guix**, so they are reproducible: anyone who builds the same version with Guix gets exactly the same files and checksums. See [CHANGELOG-community.md](CHANGELOG-community.md) for what changed in each community release.

## Build from source (Linux)

~~~
git clone https://github.com/BTGS-Community/btgs-core-old.git
cd btgs-core-old
cmake -B build
cmake --build build -j$(nproc)
~~~

The programs (`bitcoind`, `bitcoin-cli`, `bitcoin-qt`) will be in `build/bin/`. The data folder is `~/.btgs` and the config file is `btgs.conf`.

Reproducible release builds (Linux and Windows):

~~~
env HOSTS='x86_64-linux-gnu x86_64-w64-mingw32' ./contrib/guix/guix-build
~~~

See [contrib/guix/README.md](contrib/guix/README.md) for details.

## Official links

| Resource | Link |
| :--- | :--- |
| Website | [bitcoingoldbtgs.com](https://bitcoingoldbtgs.com/) |
| Block explorer | [explorer.bitcoingoldbtgs.com](https://explorer.bitcoingoldbtgs.com/) |
| GitHub | [github.com/BTGS-Community](https://github.com/BTGS-Community) |
| Wallet releases | [btgs-wallet releases](https://github.com/BTGS-Community/btgs-wallet/releases) |
| Snapshot check | [btgs-snapshot-check](https://github.com/BTGS-Community/btgs-snapshot-check) |
| Telegram | [BTGS Community](https://t.me/bitcoingoldbtgscommunity) |
| X (Twitter) | [@BTGSGOLD](https://x.com/BTGSGOLD) |

## Safety

- Only download wallets from the links above.
- Websites, web wallets, APIs, Electrum servers and mobile apps from the former developer (bitcoingold.site, btgscoin.site) are **not** run by the BTGS Community. Please don't use them.
- Never share your recovery phrase or wallet file. Staff will never DM you first.

## License

MIT License. See [COPYING](COPYING).
