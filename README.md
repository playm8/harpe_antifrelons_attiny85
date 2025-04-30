# Générateur Haute Tension DIY pour Harpe Électrique Anti-Frelons

## ⚡ Module autonome à salves contrôlées – Basé ATtiny85

Ce projet open source propose un **générateur haute tension DIY**, spécialement conçu pour être intégré dans une **harpe électrique anti-frelons**. Il offre une tension suffisante pour **engourdir les frelons asiatiques sans danger pour les abeilles**, tout en étant autonome, basse consommation et piloté intelligemment selon les conditions météo.

---

## 🎯 Finalité du projet

- Produire des **salves de haute tension (~2 000 V)** via un booster piloté
- Éviter les générateurs trop puissants conçus pour clôtures électriques (trop dangereux)
- **Sécurité des abeilles prioritaire** : intensité faible, salves brèves, déclenchement conditionnel
- Alimenté par **batterie 12 V + régulateur à 3,9 V**, avec activation automatique (soleil, pas de pluie, bonne température)

---

## ✅ Ce que ce projet **n'est pas**

- ❌ Une harpe électrique complète
- ❌ Un générateur haute tension continu ou permanent
- ❌ Un système de clôture animale (trop puissant, dangereux)

---

## ⚙️ Fonctionnement général

- Le microcontrôleur ATtiny85 vérifie la température, la lumière, et la pluie
- Si les conditions sont réunies, il commande un booster HT via optocoupleur et MOSFET
- La sortie produit de **courtes salves (~10 ms)** toutes les 500 ms pour maintenir une tension efficace sans gaspillage

---

## 🔌 Choix du générateur HT

> **⚠ Important : la tension doit engourdir, pas électrocuter !**

- **Tension cible** : 1 800 à 2 000 V
- **Intensité très faible**
- Modules recommandés :
  - Petits boosters HT (Aliexpress, 3–3.9 V d’entrée)
  - Éviter les modèles pour clôtures animales : trop puissants, dangereux, champs électromagnétiques nuisibles aux abeilles
- Modules testés :
  - Certains à 3 000 V → trop intenses
  - D'autres ont grillé rapidement : privilégier les modèles robustes avec intensité modérée

---

## 🛑 Règles de sécurité essentielles

> Ce système produit des tensions dangereuses. Respectez ces consignes impérativement.

- **Alimenter TOUT le circuit avec du 3,9 V régulé** — jamais plus de 4,2 V
- **Tester d'abord avec une LED témoin** à la place du booster HT
- **Isoler toutes connexions haute tension** (gaine thermo, colle chaude, boîtier fermé)
- **Débrancher la batterie avant toute intervention**
- **Installer une résistance de décharge (≥ 5 MΩ)** entre sortie HT et GND
- **Éviter tout contact direct avec les fils de la harpe**
- **Tenir hors de portée des enfants et animaux**

---

## 🔏 Licence

- **Code source** : [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.html)
- **Documentation et plans** : [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

---

**Un projet de playm – pour une apiculture défensive mais respectueuse.**  
*Questions ? Suggestions ? Ouvrez une issue !*
