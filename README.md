# l8db Extension-Markt

Öffentlicher Katalog der offiziell unterstützten l8db-Extensions. l8db lädt `catalog.json` aus diesem Repository und prüft jedes Paket anhand des dort angegebenen SHA-256-Hashs, bevor es deaktiviert installiert wird. Berechtigungen müssen anschließend in l8db geprüft und erteilt werden.

## Katalogformat

`catalog.json` enthält `schemaVersion: 1` und eine Liste `extensions`. Jeder Eintrag nennt ID, Name, Beschreibung, Version, Herausgeber, den relativen Paketpfad unter `packages/` und den SHA-256-Hash der Paketdatei. Die Paketmetadaten müssen mit dem Eintrag übereinstimmen.

## Jev

`packages/l8db.jev-1.0.0.l8db-extension` ist das installierbare Paket. Der Quellcode liegt unter `source/jev/`; die lokale Entwicklungsfassung im l8db-Projekt liegt direkt unter `/extention`. Details zu BYOK und den übertragenen Planmerkmalen stehen in [source/jev/README.md](source/jev/README.md).

## Passwortmanager-Sync

`packages/l8db.password-manager-1.0.0.l8db-extension` lädt und speichert l8db-Verbindungen in Keeper, Bitwarden oder 1Password über deren offizielle CLI und kann die CLIs per Button installieren. Benötigt l8db 0.7.0 oder neuer. Quellcode unter `source/password-manager/`, Details in [source/password-manager/README.md](source/password-manager/README.md).
