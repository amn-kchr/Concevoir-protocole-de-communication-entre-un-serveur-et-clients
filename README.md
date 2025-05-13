# Projet Réseau : Conception d'un Protocole de Communication Client-Serveur

## Présentation

Ce projet s'inscrit dans le cadre d'un enseignement en programmation réseau. Il vise à développer une compréhension concrète des architectures client-serveur, à travers la conception, l'implémentation et l'évolution d'un protocole de communication personnalisé. Le projet est divisé en plusieurs étapes, chacune introduisant de nouvelles complexités (multi-threading, protocoles, robustesse, etc.).

## Objectifs pédagogiques

* Maîtriser la programmation réseau en C (sockets TCP/IP)
* Comprendre la communication synchrone et asynchrone
* Implémenter un protocole client-serveur robuste
* Gérer la concurrence avec les threads
* Formaliser le protocole sous forme de RFC
* Rédiger un rapport technique et un rapport de développement

## Arborescence du projet

```
projet Réseau/
├── étape1_et_2/
│   ├── client1.c                  # Client simple (communication de base)
│   ├── server.c                   # Serveur de base (mono-client)
│   └── cahier_des_charges.docx   # Spécifications initiales du projet
│
├── etape3_Mono threads commenté/
│   └── server.c.docx              # Serveur mono-thread documenté
│
├── etape3_Multi threads commenté/
│   └── server.c.docx              # Serveur multi-thread documenté
│
├── etape 4/
│   ├── code/
│   │   ├── client.c               # Client final avec gestion du protocole
│   │   ├── serveur.c              # Serveur final multi-client
│   │   └── Makefile               # Compilation automatisée
│   ├── RFC.pdf                    # Spécification formelle du protocole
│   ├── rapport_de_developpement.pdf # Journal de développement
│   └── Rapport Technique...pdf   # Rapport final du projet
```

## Compilation

Placez-vous dans le dossier `etape 4/code` puis utilisez le Makefile :

```bash
cd "etape 4/code"
make
```

Cela génère deux exécutables : `serveur` et `client`.

## Utilisation

### Serveur

```bash
./serveur <port>
```

### Client

```bash
./client <adresse_ip> <port>
```

## Fonctionnalités principales

* Connexion de plusieurs clients simultanément (threading)
* Protocole personnalisé d'échange de messages
* Gestion d'erreurs et robustesse (timeouts, erreurs de socket)
* Structure modulaire du code
* Conformité à une RFC interne (voir `etape 4/RFC.pdf`)

## Contributions

* **KECHIR Amine**

## Documentation

* `Rapport Technique` : Détails sur la conception, les choix techniques, les tests
* `rapport_de_developpement.pdf` : Suivi de l'évolution du projet
* `RFC.pdf` : Définition formelle du protocole implémenté
* `cahier_des_charges.docx` : Expression des besoins initiale

## Licence

Ce projet est publié sous licence MIT. Vous êtes libre de le modifier et de le redistribuer sous les mêmes conditions.

---
## Auteur

[KECHIR AMINE](https://github.com/amn-kchr)
