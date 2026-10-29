# BTGS Community changelog

Community maintained builds of the BTGS node and wallet (existing chain).
Base: original BTGS source, commit 6f988e8 (Bitcoin Core 30.2 based, v30.2.3).

## v30.2.4

No changes to consensus or chain rules. Same network, same blocks, same coins.

Changes:
- New working seed nodes (the old seed servers were offline):
  rodb2008.com, 23.94.86.196, 85.190.101.78 (also built in as fixed seeds, port 18888)
- Website link now points to https://bitcoingoldbtgs.com/
- Source code and bug report links now point to https://github.com/BTGS-Community/btgs-core-old
- README rewritten for the community (old links and unverified claims removed)
- Guix: copy btgs.conf instead of bitcoin.conf when packing the release
- Guix: use the btgs-win64-setup.exe installer name for Windows
- Version bumped to 30.2.4

Builds:
- Built with Guix (reproducible). Anyone who builds this tag with Guix
  should get exactly the same files and checksums.
- Linux (x86_64) and Windows (64-bit). macOS later.

Maintained by the BTGS Community (GreenMiner).
