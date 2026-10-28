# Contrat de sous-traitance de données personnelles (article 28 RGPD)

> **PROJET — version 0.2 du 28/10/2026 — NON VALIDÉ JURIDIQUEMENT.**
> À faire relire par un avocat ou un juriste RGPD luxembourgeois avant toute signature.
> Les passages `[à compléter]`, `[À DÉCIDER]` et `[À VÉRIFIER]` doivent être résolus avant usage.
>
> **Changements par rapport à la v0.1** : corrections issues de l'analyse du 28/10/2026
> (`contrats/analyses/analyse-dpa-v0.1-hugo-salard.md`) et de la vérification des prestataires
> (`contrats/analyses/verification-prestataires-2026-10-28.md`) : interdiction des usages propres et
> de l'entraînement de modèles (art. 4), révélations spontanées et option santé (art. 2 et 10),
> transferts par prestataire avec analyse d'impact (art. 7), demandes des autorités (art. 8),
> articulation avec les CGV (art. 9), annexe 1 complétée.
> **Mise à jour du 28/10/2026** : Airtable (États-Unis) remplacé par Baserow (UE) pour le stockage.

---

**Entre**

**[Raison sociale du client]**, [forme juridique], dont le siège est situé [adresse],
immatriculée au RCS Luxembourg sous le n° [à compléter], représentée par [nom, fonction],
ci-après le **« Responsable du traitement »** ou le **« Client »**,

**et**

**AutomateLux S.à r.l.-S**, au capital de 500 €, dont le siège est situé 150, route de Fischbach,
L-7447 Lintgen, immatriculée au RCS Luxembourg sous le n° [à compléter], titulaire de
l'autorisation d'établissement n° 10194043/0, représentée par M. Nilton Soares, gérant,
ci-après le **« Sous-traitant »** ou **« AutomateLux »**.

Ce contrat complète le contrat de prestation (proposition commerciale signée et conditions
générales de vente d'AutomateLux, ci-après le « Contrat principal »). En cas de contradiction
sur la protection des données, le présent contrat prévaut.

---

## Article 1 — Objet

Le Client confie à AutomateLux la mise en place et l'exploitation d'un assistant téléphonique
automatisé (« l'Assistant ») et des automatisations associées, décrits dans le Contrat principal.
Pour exécuter ce service, AutomateLux traite des données personnelles **pour le compte et sur
instruction du Client**, au sens de l'article 28 du Règlement (UE) 2016/679 (« RGPD »).

## Article 2 — Description du traitement

| Élément | Description |
|---|---|
| Nature des opérations | Réception et prise en charge des appels entrants ; reconnaissance vocale et transcription ; génération de réponses ; enregistrement des rendez-vous ; envoi de rappels ; journalisation technique |
| Finalités | Répondre aux appels du Client lorsqu'il n'est pas disponible, prendre et gérer les rendez-vous, envoyer des rappels aux personnes qui l'ont accepté |
| Personnes concernées | Personnes qui appellent le Client (clients et prospects du Client) |
| Catégories de données | Numéro de téléphone ; nom et prénom communiqués ; date, heure et objet du rendez-vous ; contenu de la conversation (transcription) ; enregistrement audio de l'appel **[À DÉCIDER : activé ou non — recommandation : non]** ; adresse e-mail si communiquée pour un rappel |
| Données sensibles | L'Assistant n'est pas configuré pour demander de données sensibles (art. 9 RGPD). Pour les **révélations spontanées** d'un appelant, voir l'article 2.2. Pour les clients du secteur de la santé, voir l'article 10. |
| Durée du traitement | Durée du Contrat principal |
| Durée de conservation | Transcriptions : [30] jours dans le stockage désigné à l'annexe 2, puis suppression automatique. Enregistrements audio (si activés) : [30] jours. Données de rendez-vous : dans les outils du Client, selon ses règles. Journaux techniques : [90] jours. **[Durées à valider]** |

**2.2 Révélations spontanées.** Si un appelant communique de lui-même une donnée sensible, AutomateLux
ne l'utilise que dans la mesure strictement nécessaire à la prise du rendez-vous, ne la reporte pas
dans les champs du rendez-vous au-delà de ce besoin, et la supprime avec la transcription au terme
de la durée de conservation.

## Article 3 — Obligations d'AutomateLux

AutomateLux s'engage à :

1. **Instructions** : ne traiter les données que sur instruction documentée du Client, y compris
   pour les transferts hors de l'Union européenne. Le Contrat principal et le présent contrat
   constituent ces instructions. Si une instruction lui paraît contraire au RGPD, AutomateLux
   en informe immédiatement le Client.
2. **Confidentialité** : garantir que toute personne autorisée à traiter les données est soumise
   à une obligation de confidentialité.
3. **Sécurité** : mettre en œuvre les mesures de l'**Annexe 2** (article 32 RGPD).
4. **Sous-traitants ultérieurs** : respecter l'article 6.
5. **Droits des personnes** : aider le Client, dans la mesure du possible, à répondre aux demandes
   d'accès, de rectification, d'effacement, de limitation, d'opposition et de portabilité. Toute
   demande reçue directement par AutomateLux est transmise au Client sous [3] jours ouvrés.
6. **Violations de données** : notifier au Client toute violation de données personnelles **sans
   délai injustifié et au plus tard [48] heures** après en avoir pris connaissance, avec les
   informations disponibles (nature, catégories et nombre approximatif de personnes et de
   données concernées, conséquences probables, mesures prises ou proposées), puis compléter ces
   informations au fur et à mesure.
7. **Assistance** : aider le Client à respecter ses obligations de sécurité, de notification à
   la CNPD, d'information des personnes et, le cas échéant, d'analyse d'impact (articles 32 à 36).
8. **Fin du contrat** : au choix du Client, restituer ou supprimer les données dans les [30] jours
   suivant la fin du Contrat principal, y compris chez les sous-traitants ultérieurs, sauf obligation
   légale de conservation. AutomateLux confirme la suppression par écrit.
9. **Audit** : mettre à la disposition du Client les informations nécessaires pour démontrer le
   respect du présent contrat, et permettre des audits par le Client ou un auditeur mandaté,
   sur préavis écrit de [30] jours, au maximum une fois par an sauf violation avérée, aux frais
   du Client.
10. **Registre** : tenir le registre des activités de traitement effectuées pour le compte du
    Client (article 30.2 RGPD).

## Article 4 — Interdiction des usages propres et de l'entraînement de modèles

1. AutomateLux ne traite pas les données du Client pour ses propres finalités. Elle ne les vend
   pas, ne les loue pas, ne les utilise pas à des fins publicitaires ou de prospection.
2. AutomateLux **n'utilise pas les données du Client pour entraîner, ajuster ou améliorer un modèle
   d'intelligence artificielle**, ni ne l'autorise.
3. Pour chaque sous-traitant ultérieur, AutomateLux choisit les réglages qui excluent l'utilisation
   des données pour l'entraînement lorsque ce réglage existe, et documente à l'annexe 1 la position
   de chaque prestataire. **Lorsque cette position n'a pas pu être confirmée, l'annexe 1 l'indique
   expressément** ; AutomateLux s'engage à la confirmer ou à remplacer le prestataire dans un délai
   de [90] jours.
4. AutomateLux active les options de non-conservation proposées par ses prestataires lorsqu'elles
   sont compatibles avec le service (notamment l'option « Zero Data Retention » de la plateforme
   vocale, voir annexe 2).

## Article 5 — Obligations du Client

Le Client, en tant que responsable du traitement, s'engage à :

1. disposer d'une base légale pour chaque traitement confié ;
2. **informer les personnes qui l'appellent** (articles 13 et 14 RGPD) : le message d'accueil de
   l'Assistant indique qu'il s'agit d'un assistant automatisé, si l'appel est transcrit ou
   enregistré, et où trouver la notice d'information du Client (modèle fourni par AutomateLux) ;
3. recueillir et conserver le **consentement** des personnes avant l'envoi de rappels, lorsque ce
   consentement est requis ;
4. ne pas demander à AutomateLux de configurer l'Assistant pour collecter des données sensibles,
   sauf dans le cadre de l'article 10 ;
5. documenter par écrit toute instruction supplémentaire.

## Article 6 — Sous-traitants ultérieurs

1. Le Client autorise de manière générale AutomateLux à recourir aux sous-traitants ultérieurs
   listés en **Annexe 1**, avec leur identité, leur localisation, le lien contractuel et la
   garantie de transfert.
2. AutomateLux informe le Client par écrit, au moins [30] jours à l'avance, de tout ajout ou
   remplacement. **Aucun nouveau sous-traitant ne traite les données avant la fin de ce délai.**
   Le Client peut s'y opposer pour un motif légitime lié à la protection des données. À défaut
   d'accord, chaque partie peut résilier le Contrat principal sans pénalité, et les sommes payées
   d'avance pour la période non exécutée sont remboursées.
3. AutomateLux impose à chaque sous-traitant ultérieur des obligations de protection au moins
   équivalentes à celles du présent contrat (ou, pour les prestataires qui imposent leurs propres
   conditions, s'assure que ces conditions offrent des garanties équivalentes), et reste
   responsable envers le Client de leur respect.

## Article 7 — Transferts hors de l'Union européenne

1. Les transferts vers un pays hors de l'Espace économique européen ne sont effectués que vers les
   prestataires de l'annexe 1, et uniquement sur la base indiquée pour chacun :
   - la **décision d'adéquation EU-U.S. Data Privacy Framework**, lorsque le prestataire figure
     comme certifié et actif sur le registre officiel (dataprivacyframework.gov) ; ou
   - les **clauses contractuelles types** de la Commission européenne (décision 2021/914), intégrées
     au contrat du prestataire, avec le module applicable.
2. Pour chaque transfert fondé sur les clauses contractuelles types, AutomateLux réalise et tient à
   la disposition du Client une **analyse d'impact du transfert** (évaluation de la législation du
   pays de destination et des mesures complémentaires).
3. AutomateLux **vérifie au moins une fois par an** la certification des prestataires fondés sur le
   Data Privacy Framework et met l'annexe 1 à jour.
4. **Si une base de transfert disparaît** (retrait de certification, invalidation de la décision
   d'adéquation, suspension des clauses), AutomateLux en informe le Client sans délai et, dans un
   délai de [30] jours, soit met en place une autre base valable, soit cesse le transfert concerné,
   au besoin en remplaçant le prestataire.

## Article 8 — Demandes d'accès des autorités

1. Si AutomateLux ou un sous-traitant ultérieur reçoit d'une autorité publique, notamment d'un pays
   tiers, une demande d'accès aux données du Client, AutomateLux, sauf interdiction légale :
   informe le Client sans délai, vérifie la légalité de la demande, la conteste lorsqu'il existe des
   motifs sérieux, et ne communique que le minimum de données strictement requis.
2. Lorsque la loi lui interdit d'informer le Client, AutomateLux s'efforce d'obtenir la levée de
   cette interdiction et documente sa démarche.
3. AutomateLux impose ou vérifie des engagements équivalents chez ses sous-traitants ultérieurs
   établis hors de l'EEE. **[À VÉRIFIER : ce que les DPA de Vapi, OpenAI et du
   fournisseur de transcription prévoient déjà sur ce point.]**

## Article 9 — Responsabilité

1. Chaque partie est responsable des dommages causés par sa propre violation du RGPD ou du présent
   contrat, conformément à l'article 82 RGPD.
2. **Par dérogation à l'article 11 des conditions générales de vente d'AutomateLux**, la
   responsabilité d'AutomateLux au titre du présent contrat n'est pas soumise au plafond général
   des CGV. Elle est limitée à **[À DÉCIDER : montant ou formule, par exemple un multiple des
   sommes payées sur 12 mois, ou le montant couvert par l'assurance]**, sauf faute lourde ou
   intentionnelle.
3. AutomateLux maintient une assurance responsabilité civile professionnelle **[À DÉCIDER : et une
   assurance cyber]** couvrant les traitements prévus par le présent contrat, et en remet une
   attestation au Client sur demande.

## Article 10 — Option « secteur santé »

**Cette option n'est pas disponible tant qu'elle n'a pas été validée par un juriste.** Lorsque le
Client est un professionnel de santé humaine (cabinet médical, dentaire, paramédical), le motif
du rendez-vous peut constituer une donnée de santé. Avant toute mise en service, les parties
conviennent par écrit : de la base légale applicable au titre de l'article 9.2 du RGPD ; de la
désactivation de l'enregistrement audio ; d'une durée de conservation réduite des transcriptions ;
de la nécessité d'une analyse d'impact (article 35) ; et de prestataires adaptés.
*Les cabinets vétérinaires ne sont pas concernés par cet article : la santé d'un animal n'est pas
une donnée de santé au sens du RGPD.*

## Article 11 — Durée

Le présent contrat entre en vigueur à sa signature et prend fin à l'expiration du Contrat
principal. Les obligations de l'article 3.8 (restitution et suppression), de confidentialité et
de l'article 9 survivent à cette fin.

## Article 12 — Droit applicable

Droit luxembourgeois. Tribunaux compétents : ceux de Luxembourg-Ville.

---

Fait à [lieu], le [date], en deux exemplaires.

| Pour le Client | Pour AutomateLux S.à r.l.-S |
|---|---|
| [Nom, fonction] | Nilton Soares, gérant |
| Signature : | Signature : |

---

## Annexe 1 — Sous-traitants ultérieurs

Vérifications du 28/10/2026 : registre officiel du Data Privacy Framework et documentation publique
des prestataires. Les conditions réellement attachées aux comptes d'AutomateLux restent à confirmer
(colonne « Lien contractuel »).

| Prestataire | Rôle | Lien contractuel | Lieu de traitement | Garantie de transfert | Entraînement de modèles sur les données |
|---|---|---|---|---|---|
| Superpowered Inc. (**Vapi**), États-Unis | Plateforme de l'agent vocal | Direct — DPA intégré aux conditions d'utilisation de Vapi | États-Unis | Clauses contractuelles types + analyse d'impact | **Non confirmé** — à confirmer (art. 4.3) |
| **OpenAI Ireland Ltd**, Irlande (clé API d'AutomateLux) | Génération des réponses (modèle GPT-4.1) | Direct — DPA OpenAI **[à confirmer : accepté dans le compte]** | États-Unis (traitement par OpenAI OpCo, LLC) | Clauses contractuelles types + analyse d'impact | **Non** par défaut pour l'API (documentation OpenAI) |
| **ElevenLabs** (clé API d'AutomateLux) | Synthèse vocale | Direct — DPA ElevenLabs **[à confirmer selon l'offre]** | États-Unis | **Data Privacy Framework** — certification active vérifiée le 28/10/2026 | **Non confirmé** — à confirmer (art. 4.3) |
| **[Fournisseur de transcription — à confirmer dans le compte Vapi]** | Reconnaissance vocale | [Direct (clé API d'AutomateLux) / via Vapi — à confirmer] | [à compléter] | [à compléter — ex. Deepgram : non certifié DPF, clauses contractuelles types à vérifier] | **Non confirmé** |
| **[Opérateur téléphonique — à confirmer]** (ex. Twilio Inc.) | Numéro et acheminement des appels | [à confirmer] | [à compléter] | Si Twilio : **Data Privacy Framework** — certification active vérifiée le 28/10/2026 | Sans objet |
| **Celonis (Make.com)** | Automatisations (webhooks) | Direct — DPA Make | Union européenne (région EU1) **[à confirmer]** | Hébergement UE ; Celonis Inc. certifiée DPF (vérifié le 28/10/2026) | **Non confirmé** |
| **Baserow** B.V., Pays-Bas | Stockage des rendez-vous et des transcriptions | Direct — DPA Baserow **[à accepter dans le compte]** | Union européenne (Allemagne) — VÉRIFIÉ (documentation Baserow) | Sans objet (UE) ; **[À VÉRIFIER : identité de l'hébergeur et éventuels sous-traitants hors UE]** | **Non confirmé** |
| **Brevo** (Sendinblue SAS), France | Envoi des rappels par e-mail / SMS | Direct — DPA Brevo | Union européenne **[à confirmer]** | Sans objet si UE | **Non confirmé** |

## Annexe 2 — Mesures de sécurité (article 32 RGPD)

> Ne laisser dans cette liste que ce qui est **réellement en place** à la date de signature.

- **Zero Data Retention activé sur la plateforme vocale (Vapi)** : aucun enregistrement, transcription
  ni résumé n'est conservé par Vapi après l'appel ; seules des métadonnées techniques et de
  facturation sont conservées.
- Rendez-vous et transcriptions conservés uniquement dans **Baserow, hébergé dans l'Union
  européenne (Allemagne)**.
- Accès aux comptes des prestataires protégés par mot de passe unique et authentification à deux facteurs.
- Accès limité au gérant d'AutomateLux ; aucun partage d'identifiants.
- Chiffrement des échanges (HTTPS/TLS) entre les services.
- Clés d'API conservées hors des documents partagés, renouvelées en cas de doute.
- Suppression automatique des transcriptions et enregistrements au terme de la durée de l'article 2.
- Un espace de données séparé par client.
- Procédure de notification des violations : voir article 3.6.
- Retour automatique des appels vers la messagerie habituelle du Client en cas de panne.
