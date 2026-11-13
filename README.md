# ToIP Asterisk sur AWS

Déploiement d'un IPBX Asterisk sur une instance AWS EC2 (Ubuntu Server),
avec SIP/PJSIP, RTP, IVR et protection anti-scanners.

## Objectif
Mettre en place une téléphonie sur IP accessible depuis des softphones, sur
une infrastructure cloud, et documenter l'installation de bout en bout.

## Contexte
TP Téléphonie sur IP, Master 2 SRT (ESP/UCAD), 2024-2025.
Encadrant : Dr Moustapha Mbaye.

## Architecture
- Cloud : AWS EC2 Free Tier, Ubuntu Server 24.04 LTS
- IPBX : Asterisk 20 (compilé depuis les sources)
- Signalisation : SIP / PJSIP (RFC 3261), transport RTP/RTCP
- Softphone : Linphone ; IVR via synthèse vocale ; Fail2ban anti-scanners SIP

## Contenu
- `config/` : `pjsip.conf` et `extensions.conf` (identifiants et IP **remplacés par des placeholders**)
- `docs/` : rapport, guide d'installation et source LaTeX

## Sécurité
Les mots de passe SIP et l'adresse IP publique ont été remplacés par des
placeholders (`<MOT_DE_PASSE>`, `<IP_PUBLIQUE>`). Remplace-les par tes
propres valeurs avant tout déploiement. Ne jamais committer de vraies clés.

## Licence
MIT (code/config) — voir `LICENSE`. Documents : contenu rédactionnel.
