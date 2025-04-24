# MiniLab Packet Tracer – MSc Cybersécurité

## 🔎 Objectif
Ce projet a pour but de créer un mini-laboratoire réseau simulé dans Cisco Packet Tracer pour valider les compétences techniques en réseaux dans le cadre du test d'admission au MSc Cybersécurité de Cybersup.

## 🛠ï Architecture
Le réseau est composé de 3 bureaux interconnectés, chacun avec :
- 1 switch
- 1 point d'accès Wi-Fi
- 1 PC portable
- 2 PC fixes
- 1 téléphone IP
- 1 PC administration

Le tout connecté à un routeur Cisco 1941 configuré pour :
- Le routage inter-VLAN
- Le serveur DHCP
- La passerelle Internet simulée

## 📂 VLANs et Plan IP
| VLAN | Rôle | Adresse Réseau | Gateway | Plage DHCP |
|------|------|------------------|---------|-------------|
| 1    | VoIP | 192.168.0.0/24   | .1      | .10-.50     |
| 10   | Wi-Fi | 192.168.10.0/24 | .1      | .10-.50     |
| 20   | PC fixes | 192.168.20.0/24 | .1   | .10-.50     |
| 30   | Admin | 192.168.30.0/24 | .1      | .10-.50     |

## ⚙️ Configuration effectuée
- VLANs créés sur chaque switch
- Ports configurés en access ou trunk selon la fonction
- Routeur configuré avec sous-interfaces (dot1Q)
- DHCP configuré pour chaque VLAN
- Tests de connectivité réalisés (ping inter-VLAN)

## 📷 Captures d'écran fournies
- Vue de la topologie
- Affectation VLAN sur un switch
- Configuration routeur (sous-interfaces, DHCP)
- Attribution IP automatique (DHCP)
- Ping inter-VLAN

## 📁 Fichiers inclus
- `MiniLab.pkt` : projet Packet Tracer
- `Documentation.pdf` : guide de réalisation du lab
- `config_routeur.txt` et `config_switchX.txt` : exports CLI (facultatif)
- Ce fichier `README.md`

## 🚀 Auteur
Ruben Arnald Hombessa Massamouna

---
Projet réalisé dans le cadre du test d'admission au MSc Cybersécurité de Cybersup.
