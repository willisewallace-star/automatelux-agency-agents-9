# Contexte AutomateLux — référence commune des agents

Faits stables uniquement. Aucun état de pipeline, aucun client en cours, aucun chiffre
de prospection : ces données vieillissent vite et doivent être demandées au gérant.

Niveaux de confiance utilisés : **VÉRIFIÉ** (document officiel), **PROBABLE**,
**ESTIMÉ** (ordre de grandeur), **À VÉRIFIER** (contradiction ou doute connu).

---

## Société

| Champ | Valeur |
|---|---|
| Raison sociale | AutomateLux S.à r.l.-S |
| Gérant unique | Nilton Soares |
| Siège | 150, route de Fischbach — L-7447 Lintgen — Luxembourg |
| Capital | 500 € |
| Constitution | 25/03/2025 |
| Autorisation d'établissement | Réf. 10194043/0 — Ministère de l'Économie — 24/04/2026 |
| Site | automatelux.com |
| Statuts | Version V4 définitive — ne pas proposer de les modifier |

Langues : français (principal), luxembourgeois et anglais (secondaires).
Ressources : gérant seul, temps partiel (~20 h/semaine), budget de départ très serré
(~500 €), acquisition organique en priorité.

### Gérant légal et nom commercial

- **Nilton Soares est le seul gérant** : RCS, statuts, autorisation, contrats, factures,
  signatures, banques, administrations. Partout où une personne engage la société, c'est lui.
- **« Léon » est un prénom commercial fictif** (persona de prospection et de contact), au
  même titre que « Claude » ou « Marie ». Il peut signer un e-mail de prospection
  (« Léon — AutomateLux ») et utiliser l'adresse `leon@automatelux.com`.
- « Léon » ne porte **jamais** le titre de gérant, ne signe **jamais** un contrat, une
  proposition engageante ou une facture, et n'apparaît dans aucun document officiel.
- Si un prospect ou un client demande à qui il parle, ne pas mentir : orienter vers Nilton
  Soares. Si « Léon » est la voix d'un agent IA, elle doit s'annoncer comme automatisée.

E-mail de contact commercial : `leon@automatelux.com`. Téléphone : ne jamais l'inventer,
écrire `[téléphone à compléter]`.

---

## Activité 1 — Agence d'automatisation IA pour PME

Automatiser les tâches répétitives des PME luxembourgeoises : répondre aux appels,
prendre les rendez-vous, relancer les clients.

**Pitch** : zéro appel manqué, le gérant se concentre sur son métier, opérationnel en 7 jours.

**Stack** : Make.com (région EU1), Vapi (agent vocal, voix ElevenLabs), Airtable, Brevo
(e-mailing), Hostinger (domaine), Outscraper (extraction de prospects), Lovable (sites).

### Offres

| Offre | Mise en place | Mensuel | Cible |
|---|---|---|---|
| Starter | 1 500 € | 400 €/mois | Salons, petits cabinets |
| Pro | 2 500 € | 800 €/mois | Dentistes, avocats |
| Elite | 4 000 € | 1 500 €/mois | Multi-sites, groupes |

Cibles prioritaires : salons de coiffure (Luxembourg-Ville, Esch, Differdange),
vétérinaires / cliniques animales, cabinets notariaux juniors.

### Livraison type (7 jours)

```
J1   Kickoff 30 min + collecte des accès (numéro, agenda, logo, langue)
J2-3 Configuration Vapi + webhook Make.com + Airtable
J4   Tests internes (10 appels simulés)
J5   Formation client 1 h
J7   Mise en ligne + point de contrôle
J30  Bilan + upsell éventuel + demande de recommandation
```

### Règles commerciales non négociables

- **Acompte de 50 % avant tout démarrage.** Zéro travail sans virement reçu.
- **Pas d'achat de matériel avant le premier client payant.**
- **Facturation** : mention « TVA non applicable — article 57 de la loi TVA
  luxembourgeoise » tant que le chiffre d'affaires reste sous le seuil de franchise.
  Seuil indiqué : 50 000 €/an — **PROBABLE, à reconfirmer auprès de l'AED** (le seuil a
  changé récemment).
- Parler des problèmes de la PME, jamais de la technologie. Pas de jargon IA.

---

## Activité 2 — Automates en libre-service

Couverte par l'objet social (laveries, stations de lavage, distributeurs, mobilité
électrique en libre-service).

### Machines étudiées (ordres de grandeur, ESTIMÉ sauf mention)

| Machine | Investissement | Prix / usage | ROI annoncé |
|---|---|---|---|
| Station de lavage auto | 30–80 k€ machine + 15–40 k€ installation | 6–15 € | 3–6 ans (PROBABLE) |
| Aspirateur auto | 1,5–4 k€ | 1–3 € | 6–18 mois (PROBABLE) — rarement viable seul |
| Lave-tapis auto | 8–20 k€ | 3–6 € | 2–4 ans (PROBABLE) |
| Distributeur café | 3–15 k€ | 0,80–2,50 € | 1–3 ans (PROBABLE) — marché saturé |
| Distributeur glace / frais | 5–15 k€ | 1–5 € | Inconnu — saisonnalité forte |
| Nettoyage vapeur casques / EPI | 3–8 k€ | 3–8 € | Inconnu — marché probablement trop petit |

### Règles de rentabilité

- Loyer ou commission terrain ≤ 20 % du CA prévisionnel (préférer 15–25 % du CA au loyer fixe au démarrage).
- Eau + électricité : 15–25 % du CA. Maintenance : réserver 5–10 % du CA chaque mois.
- Objectif : marge nette ≥ 30 % après charges.
- Séquence : machine pilote bon marché → 3 mois de données réelles → réinvestir.
- Ne jamais signer un emplacement sans comptage de flux réel sur place.

```
CA mensuel   = Prix × Cycles/jour × 30
Marge nette  = CA − (eau + élec + consommables) − (loyer + maintenance + assurance)
ROI (mois)   = Investissement total / Marge nette mensuelle
```

### Cadre légal (à confirmer avant tout achat)

- Alimentaire (café, glace) : hygiène HACCP, contrôles de l'ALVA (Administration
  luxembourgeoise vétérinaire et alimentaire), carnet de nettoyage.
- Lavage auto : séparateur d'hydrocarbures obligatoire, conformité Administration de
  l'environnement, permis de construire possible.
- Assurances : RC exploitation, bris de machine, protection juridique.

**À VÉRIFIER — tension entre les deux activités** : la règle « pas de matériel avant le
premier client payant » vient de l'activité agence. Une machine en libre-service est un
investissement matériel par nature. Ne pas trancher à la place du gérant : signaler le
conflit dès qu'un achat de machine est envisagé.

---

## Règles pour tous les agents

1. Répondre en français, sauf demande contraire.
2. Distinguer les faits (ce fichier) des estimations. Jamais présenter un chiffre ESTIMÉ comme certain.
3. Ne jamais inventer un client, un témoignage, un chiffre de résultat ou une référence.
   Pour une preuve sociale, demander au gérant ce qui est réel et autorisé.
4. Toute donnée datée (clients, pipeline, trésorerie, contacts) : la demander, ne pas la supposer.
5. Signaler un risque juridique (RGPD, TVA, hygiène, environnement) dès qu'il apparaît,
   sans se faire passer pour un juriste ou un comptable agréé.
