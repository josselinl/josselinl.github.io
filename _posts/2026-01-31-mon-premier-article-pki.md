---
layout: post
title:  "Bienvenue sur mon blog PKI !"
date:   2026-01-31 00:15:00 +0100
categories: pki introduction
tags: [pki, chiffrement, blog]
---

# Mon expertise PKI en quelques mots

Bonjour ! Expert **PKI** avec X ans d'expérience en :
- Déploiement d'infrastructures à clé publique
- Gestion HSM (Thales, Yubico...)
- Intégration KMS cloud/on-prem

## Pourquoi ce blog ?
Partager mes retours d'expérience techniques sur :
- Meilleures pratiques PKI
- Troubleshooting certificats
- Sécurité chiffrement moderne

## Premier tip PKI
**Vérifier expiration CA** :
```bash
openssl x509 -in cert.pem -noout -dates
