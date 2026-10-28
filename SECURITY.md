# Security & Cryptographic Identity

## ⚠️ KRYPTOGRAFISCHE MIGRATION (DEPRECATION NOTICE)
**Datum der Umstellung:** 28. Oktober 2026

Hiermit dokumentiere ich den offiziellen Wechsel der kryptografischen Architektur für dieses Projekt und meine Entwickler-Identität.

### 1. Der alte Anker: PGP (Verworfen)
Der bisherige GPG/PGP-Schlüssel wird ab sofort **nicht mehr verwendet** (Status: Deprecated / Verworfen). 
*Grund:* PGP ist ein historisch gewachsenes System aus den 90er Jahren. Es ist komplex, schwerfällig und erfordert unnötigen Overhead (Key-Server, Web of Trust-Inseln, große Schlüsseldateien). Der alte Schlüssel ist nicht kompromittiert, entspricht aber nicht mehr den Zero-Trust- und Minimalismus-Prinzipien (Proof of Minimalism) dieses Projekts.

### 2. Der neue Genesis-Anker: W3C DID (Ed25519)
Ab sofort wird für alle Signaturen, Releases und Attestierungen ausschließlich moderne, elliptische Kurven-Kryptografie (Ed25519) via `minisign` verwendet. Die Identität wird auf das globale W3C-Protokoll für Decentralized Identifiers (DID) umgestellt.

**Die neue, alleingültige Identität lautet:**
`did:key:z6Mkfw3iLzZZ5H7jsRKs9fx1x9Ve4AcMNQjor3KCY216P8fa`

**Der dazugehörige Public Key (Minisign) lautet:**
`RWQwc2lrky6VsRX6AYWDkxqmRYpfMi81KqJpp04rN//4q2ooakenkuA5`

### 3. Verifikation künftiger Releases
Alle künftigen Releases (wie die HAFÜDAT-Kernlogik) werden ausschließlich mit diesem neuen Ed25519-Schlüssel signiert. Die Verifikation erfolgt nicht mehr über GnuPG, sondern lokal und offline über Minisign.

*Diese Deklaration markiert den kryptografischen Genesis-Block der neuen Architektur.*
