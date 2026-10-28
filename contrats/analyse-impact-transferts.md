# Analyse d'impact des transferts de données vers les États-Unis (TIA)

> **PROJET — version 0.1 du 28/10/2026 — NON VALIDÉ JURIDIQUEMENT.**
> Document interne d'AutomateLux S.à r.l.-S, exigé par l'article 7.2 du contrat de sous-traitance
> (v0.2) et par la clause 14 des clauses contractuelles types 2021/914. Méthode : les six étapes
> des **recommandations 01/2020 du Comité européen de la protection des données (EDPB)**.
> À faire relire par un juriste. À mettre à jour au moins une fois par an et à chaque événement
> listé à l'étape 6.
>
> Niveaux de confiance : **VÉRIFIÉ** (source consultée le 28/10/2026), **PROBABLE**,
> **À VÉRIFIER** (dépend des comptes d'AutomateLux ou d'une information non trouvée).

---

## Étape 1 — Cartographie des transferts

**Exportateur** : AutomateLux S.à r.l.-S, sous-traitant de ses clients (salons, restaurants, cabinets).
**Personnes concernées** : personnes qui appellent les clients d'AutomateLux.
**Données** : numéro de téléphone, prénom/nom, date/heure/objet du rendez-vous, contenu de la
conversation (audio en temps réel, transcription). Pas d'enregistrement audio conservé (recommandé).
Données sensibles : non recherchées ; **révélations spontanées possibles** (ex. santé).

| Destinataire | Rôle | Données reçues | Durée de présence aux États-Unis | Base de transfert |
|---|---|---|---|---|
| Vapi (Superpowered Inc.) | Plateforme vocale | Audio en temps réel, transcription, métadonnées | Pendant l'appel ; **avec Zero Data Retention : pas de conservation du contenu après l'appel** (métadonnées de facturation conservées) | **Clauses contractuelles types** (non certifié DPF — VÉRIFIÉ) |
| OpenAI (via OpenAI Ireland Ltd ; traitement par OpenAI OpCo, LLC) | Génération des réponses | Texte de la conversation | Conservation **jusqu'à 30 jours** pour la détection d'abus ; **aucune** si Zero Data Retention accordé — VÉRIFIÉ | **Clauses contractuelles types** (non certifié DPF — VÉRIFIÉ) |
| Fournisseur de transcription **[à confirmer — Deepgram ?]** | Reconnaissance vocale | Audio en temps réel | **À VÉRIFIER** | **À VÉRIFIER** (Deepgram : non certifié DPF — VÉRIFIÉ) |
| Airtable (Formagrid Inc.) | Stockage des rendez-vous | Nom, téléphone, rendez-vous | Durée du contrat | **Clauses contractuelles types** (non certifié DPF — VÉRIFIÉ) |
| ElevenLabs | Synthèse vocale | Texte des réponses de l'assistant (peut contenir prénom, date) | **À VÉRIFIER** | **Data Privacy Framework** — certification active (VÉRIFIÉ) : **pas de TIA requise**, voir étape 3.4 |
| Twilio (si utilisé) | Téléphonie | Numéro, flux audio | — | **Data Privacy Framework** — certification active (VÉRIFIÉ) : **pas de TIA requise** |

**Transferts couverts par la présente analyse** : Vapi, OpenAI, Airtable et le fournisseur de transcription.

## Étape 2 — Outil de transfert

Clauses contractuelles types 2021/914, **module 3 (sous-traitant vers sous-traitant)**, intégrées aux
contrats de traitement de données (DPA) de Vapi, OpenAI et Airtable. **[À VÉRIFIER pour chacun :
module effectivement retenu et acceptation du DPA dans le compte d'AutomateLux. Pour OpenAI, le
cocontractant d'un client de l'EEE est OpenAI Ireland Ltd — VÉRIFIÉ.]**

## Étape 3 — Évaluation du droit et des pratiques des États-Unis

### 3.1 Lois susceptibles de permettre un accès aux données

- **Section 702 du FISA** (collecte de renseignement visant des personnes non américaines, auprès
  des « fournisseurs de services de communications électroniques », catégorie qui inclut
  **probablement** les fournisseurs de cloud et d'IA comme Vapi, OpenAI et Airtable).
  **Situation au 28/10/2026** : la loi n'a pas été reconduite par le Congrès et **a expiré en juin
  2026**, mais **la collecte se poursuit jusqu'en mars 2027** sur la base d'une décision de la
  cour FISC du 17 mars 2026, qui n'a pas été déclassifiée — VÉRIFIÉ (presse spécialisée, octobre 2026).
- **Executive Order 12333** (renseignement hors du territoire, sans contrainte sur le fournisseur).
- **CLOUD Act** (accès des autorités judiciaires américaines aux données détenues par un fournisseur
  américain, y compris hors des États-Unis).

### 3.2 Garanties existantes

- **Executive Order 14086** (octobre 2022) : principes de nécessité et de proportionnalité pour le
  renseignement, et voie de recours (Civil Liberties Protection Officer, puis **Data Protection
  Review Court**). Selon la Commission européenne, ces garanties s'appliquent **à tous les
  transferts vers les États-Unis, quel que soit l'outil de transfert**, y compris les clauses
  contractuelles types — VÉRIFIÉ (position de la Commission rapportée par des sources juridiques ;
  à confirmer dans le texte officiel).
- **Décision d'adéquation du 10/07/2023** (Data Privacy Framework), qui conclut que le niveau de
  protection américain est adéquat pour les entreprises certifiées. **Recours rejeté par le
  Tribunal de l'UE le 3 septembre 2025 (affaire T-553/23, Latombe) ; pourvoi pendant devant la
  Cour de justice (affaire C-703/25 P, introduit le 31 octobre 2025)** — VÉRIFIÉ.

### 3.3 Fragilités identifiées

- **Organe de contrôle (PCLOB)** : trois de ses membres ont été révoqués le 27 janvier 2025, ce qui
  lui a fait perdre son quorum — VÉRIFIÉ. Le rétablissement du quorum au 28/10/2026 n'a **pas pu
  être confirmé**. Or la Commission s'appuie sur ce contrôle pour surveiller l'application de
  l'EO 14086.
- **Décision FISC du 17 mars 2026 non déclassifiée** malgré l'échéance légale, selon des sénateurs
  américains — VÉRIFIÉ (presse). Elle empêche d'évaluer comment la collecte est encadrée en pratique.
- **Pourvoi C-703/25 P** : la Cour de justice a déjà invalidé deux cadres précédents (Safe Harbor en
  2015, Privacy Shield en 2020). Une invalidation affaiblirait aussi l'analyse des transferts sous
  clauses contractuelles types, puisque les garanties de l'EO 14086 en sont le socle commun.

### 3.4 Transferts fondés sur le Data Privacy Framework (ElevenLabs, Twilio)

Ils n'exigent pas d'analyse d'impact tant que la décision d'adéquation est en vigueur et que la
certification est active. Ils sont toutefois exposés au même risque d'invalidation (étape 6).

### 3.5 Probabilité concrète d'accès

| Facteur | Appréciation |
|---|---|
| Nature des données | Faible sensibilité : rendez-vous de salon, de restaurant. **Élevée** si un client est un cabinet de santé humaine. |
| Intérêt pour un service de renseignement | **Faible** (PROBABLE) : petites entreprises luxembourgeoises sans lien avec la sécurité nationale ou le terrorisme. Cela n'exclut pas une collecte de masse ou par sélecteurs larges. |
| Volume | Faible (quelques centaines à milliers d'appels par mois). |
| Durée d'exposition | Réduite pour Vapi (Zero Data Retention) et OpenAI (30 jours, 0 avec ZDR). **Longue pour Airtable** (stockage permanent des rendez-vous). |
| Demandes déjà reçues par les prestataires | **À VÉRIFIER** : rapports de transparence de Vapi, OpenAI, Airtable et du fournisseur de transcription. |

**Conclusion de l'étape 3** : le droit américain permet un accès plus large que ce qu'admet le droit
de l'UE, mais les garanties de l'EO 14086 s'appliquent et ont été jugées suffisantes par la
Commission et, en première instance, par le Tribunal de l'UE. Ces garanties sont **fragiles**
(contrôle affaibli, base légale de la section 702 en suspens, pourvoi pendant). Des mesures
complémentaires sont donc nécessaires, en priorité la **réduction des données transférées**.

## Étape 4 — Mesures complémentaires

### 4.1 Limites des mesures techniques

L'assistant vocal doit traiter la conversation **en clair** chez Vapi, chez le fournisseur de
transcription et chez OpenAI pour fonctionner. Selon les recommandations 01/2020 de l'EDPB, le
chiffrement ne protège pas contre un accès des autorités lorsque le prestataire doit traiter les
données en clair. **Aucune mesure technique ne neutralise entièrement le risque pour ces trois
prestataires.** La protection repose sur la minimisation et la durée d'exposition.

### 4.2 Mesures retenues

| # | Mesure | Prestataire | Effet | Statut |
|---|---|---|---|---|
| M1 | Activer **Zero Data Retention** de Vapi | Vapi | Plus aucun contenu d'appel conservé aux États-Unis après l'appel | **À FAIRE** (gratuit) |
| M2 | Demander le **Zero Data Retention** à OpenAI pour le compte d'AutomateLux | OpenAI | Supprime la conservation de 30 jours | **À FAIRE** (sur demande, accord non garanti) |
| M3 | **Remplacer Airtable par un stockage situé dans l'UE** pour les rendez-vous et transcriptions | Airtable | **Supprime le transfert le plus long** | **RECOMMANDÉ** — choix du prestataire à faire |
| M4 | Pas d'enregistrement audio | Tous | Moins de données sensibles et identifiantes | Recommandé dans le contrat (art. 2) |
| M5 | Consignes à l'assistant : ne pas demander le motif détaillé ni de données de santé ; ne pas reprendre les révélations spontanées | Tous | Minimisation | **À FAIRE** dans la configuration |
| M6 | Transcriptions conservées [30] jours au maximum, puis suppression | Stockage | Exposition réduite | Prévu au contrat |
| M7 | Chiffrement en transit (TLS) et comptes protégés par double authentification | Tous | Protège contre les tiers non étatiques | **À VÉRIFIER** dans chaque compte |
| M8 | Demander à chaque prestataire s'il a reçu des demandes d'autorités (section 702, CLOUD Act) et ses engagements de contestation | Vapi, OpenAI, transcription | Mesure contractuelle et organisationnelle | **À FAIRE** — questionnaire ci-dessous |
| M9 | **Exclure le secteur de la santé humaine** tant que la chaîne comporte des prestataires américains | Tous | Évite le cas où le risque devient élevé | Prévu (art. 10 du contrat : option bloquée) |

### 4.3 Questionnaire à envoyer aux prestataires (M8)

1. Êtes-vous, selon vous, un « electronic communication service provider » au sens de 50 U.S.C. § 1881(b)(4) ?
2. Avez-vous reçu, depuis 2023, des demandes d'accès d'autorités américaines visant des données de clients européens ? Publiez-vous un rapport de transparence ?
3. Vous engagez-vous à informer vos clients d'une telle demande lorsque la loi le permet, et à la contester lorsqu'elle est infondée ?
4. Où les données sont-elles traitées et conservées, et pendant combien de temps ?
5. Les données des clients servent-elles à entraîner ou améliorer vos modèles ? Comment l'exclure ?

## Étape 5 — Étapes procédurales

- Accepter et archiver les DPA (avec clauses contractuelles types) de Vapi, OpenAI, Airtable et du
  fournisseur de transcription, avec leur date. **À FAIRE.**
- Informer les clients de la liste des prestataires et des bases de transfert (annexe 1 du contrat).
- Conserver la présente analyse et la tenir à la disposition des clients et de la CNPD.

## Étape 6 — Réévaluation

Réévaluer **au moins une fois par an**, et immédiatement en cas de :
- **arrêt de la Cour de justice dans l'affaire C-703/25 P** (Data Privacy Framework) ;
- reconduction, modification ou fin de la section 702 du FISA (et à l'expiration de la décision FISC en mars 2027) ;
- modification ou retrait de l'EO 14086, ou évolution du contrôle par le PCLOB ;
- changement de prestataire, de localisation ou de conditions d'un prestataire ;
- arrivée d'un client du secteur de la santé humaine.

## Conclusion

| Transfert | Conclusion au 28/10/2026 |
|---|---|
| **Vapi** | **Acceptable sous condition** d'activer Zero Data Retention (M1) et d'appliquer M4, M5, M8. |
| **OpenAI** | **Acceptable sous condition** : M5 et M8 ; M2 fortement recommandé. Pas d'entraînement sur les données de l'API par défaut — VÉRIFIÉ. |
| **Fournisseur de transcription** | **Non concluable** tant que le prestataire, sa localisation et son DPA ne sont pas confirmés. |
| **Airtable** | **Risque résiduel le plus élevé** (conservation longue). **Recommandation : remplacer par un stockage dans l'UE (M3).** À défaut : acceptable à titre transitoire avec M6 et M8. |
| **Secteur santé humaine** | **Non acceptable** avec la chaîne actuelle (M9). |

**Risque résiduel global** : **modéré à faible** pour des données de rendez-vous peu sensibles, une
fois M1, M3, M4 et M5 en place. Ce risque dépend fortement de l'issue du pourvoi C-703/25 P.

Établi par : AutomateLux S.à r.l.-S — Nilton Soares, gérant — le [date de validation].

---

### Sources consultées le 28/10/2026

- Registre du Data Privacy Framework (dataprivacyframework.gov) : Vapi, OpenAI, Airtable/Formagrid, Deepgram non trouvés ; ElevenLabs, Celonis, Twilio certifiés actifs.
- docs.vapi.ai : pages « GDPR Compliance » et « Zero Data Retention ».
- developers.openai.com : « Data controls in the OpenAI platform » ; openai.com : DPA (OpenAI Ireland Ltd pour l'EEE).
- airtable.com : DPA et FAQ sur la résidence des données.
- EUR-Lex : pourvoi C-703/25 P (Latombe c. Commission), introduit le 31/10/2025, contre l'arrêt T-553/23 du 3/09/2025.
- CDT, Lawfare : révocation de membres du PCLOB le 27/01/2025.
- Computer Weekly, Wired, Brennan Center : expiration de la section 702 en juin 2026, collecte prolongée jusqu'en mars 2027 par une décision FISC du 17/03/2026.
- Commission européenne, questions-réponses sur les clauses contractuelles types (clause 14, éléments de l'analyse).
