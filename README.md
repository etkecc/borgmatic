# borgmatic

borgmatic is simple, configuration-driven backup software for servers and workstations. Protect your files with client-side encryption. Backup your databases too. Monitor it all with integrated third-party services.

[Website](https://torsion.org/borgmatic/)

[Source code](https://projects.torsion.org/borgmatic-collective/borgmatic)

# Supported Postgres versions

This image uses Alpine Linux packages for the Postgres client.
If there is no Alpine package for a specific Postgres version, that version cannot be supported by this image.

Do not open an issue requesting support for a Postgres version that is not available as an Alpine package,
it will be closed without further notice.

## How to check if a Postgres version is available as an Alpine package

Search it on [pkgs.alpinelinux.org](https://pkgs.alpinelinux.org/packages), example for Postgres 18:
[https://pkgs.alpinelinux.org/packages?name=postgresql18-client&branch=edge](https://pkgs.alpinelinux.org/packages?name=postgresql18-client&branch=edge). If you see `No matching packages found...`, then there is no Alpine package for Postgres 18.

# docker image tags

Each tag follows the scheme: `<postgres version>-<borg version>-<borgmatic version>`, thus `15-1.2.3-1.7.5` means Postgres client v15, BorgBackup v1.2.3, Borgmatic v1.7.5

The `latest` tag has the latest stable postgres client version
