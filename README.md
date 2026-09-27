# Blazing PS5 payloads

A PS5 Payload Manager (itsPLK pldmgr) repository. Every file here was taken
from its author's own GitHub release (or, for Drakmor's Discord-only builds and
Twiso's PS5SXHelper, from the copies we ran), checked to be a real ELF, and
listed with its SHA-256 so the manager verifies it on install.

Add in Payload Manager -> Settings -> Manage Sources -> Add Source:

    https://raw.githubusercontent.com/Kaoz625/blazing-ps5-payloads/main/payloads.json

Categories:
1. Boot list - add these (websrv, klogsrv, shsrv, web file manager + 7zip, PS5SXHelper)
2. Tools - load when needed
3. Controllers and audio
4. FPKG - test ALONE after a full restart (A53 PPR, one kstuff only)

`homebrew/` holds websrv homebrew apps (dump_installer, dump_runner, OffAct).
Those start from websrv's page (port 8080), not from the Payload Manager:
copy a folder into /data/homebrew/ (dump_runner goes inside a dumped game's folder).

Rule: one tool per job. One kstuff, one FTP server, one package installer.
