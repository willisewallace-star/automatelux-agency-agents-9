# Vérification des prestataires — 28/10/2026

Sert à compléter l'annexe 1 du contrat de sous-traitance (v0.2).
**DPF** = EU-U.S. Data Privacy Framework (décision d'adéquation du 10/07/2023).
**CCT** = clauses contractuelles types 2021/914.

Registre DPF interrogé le 28/10/2026 (dataprivacyframework.gov, 7 623 participants).

| Prestataire | Rôle | Certification DPF (registre officiel) | Mécanisme de transfert | Utilisation des données pour entraîner l'IA | Conservation / options | Source et confiance |
|---|---|---|---|---|---|---|
| **Vapi** (Superpowered Inc.) | Plateforme vocale | **Non trouvé** (« Vapi », « Superpowered ») | CCT, DPA intégré aux conditions d'utilisation ; traitement principalement aux États-Unis | Non vérifié | **Zero Data Retention** activable gratuitement dans le tableau de bord : aucun enregistrement, transcription ni résumé conservé après l'appel (métadonnées de facturation conservées). Région UE seulement avec l'offre Premier (sur devis) | docs.vapi.ai (GDPR, Zero Data Retention) — VÉRIFIÉ ; région UE : source tierce (echocall.de, 09/10/2026) — PROBABLE |
| **OpenAI** (modèle GPT-4.1) | Génération des réponses | **Non trouvé** (« OpenAI », « Open AI ») | CCT 2021 dans le DPA ; pour un client établi dans l'EEE, le cocontractant est **OpenAI Ireland Ltd** | **Non par défaut** pour l'API | Conservation 30 jours pour la détection des abus ; « Zero Data Retention » possible sur demande pour les points d'accès éligibles | developers.openai.com (Data controls) — VÉRIFIÉ ; OpenAI Ireland : openai.com DPA — VÉRIFIÉ |
| **ElevenLabs** | Synthèse vocale | **Certifié, actif** (UE-US, Suisse, Royaume-Uni ; données RH et non RH) | DPF ; DPA public avec CCT en complément | Non vérifié | Résidence des données dans l'UE réservée à l'offre Enterprise | Registre DPF n° 9996 — VÉRIFIÉ ; elevenlabs.io (DPA, data residency) — VÉRIFIÉ |
| **Airtable** (Formagrid Inc.) | Stockage des rendez-vous | **Non trouvé** (« Airtable », « Formagrid ») | CCT intégrées au DPA | Non vérifié | Résidence UE annoncée (FAQ) ; offre concernée non vérifiée | airtable.com (DPA, FAQ résidence) — VÉRIFIÉ ; accès au DPA selon l'offre — À VÉRIFIER |
| **Make.com** (Celonis) | Automatisations | **Celonis Inc. certifié, actif** | Hébergement UE (région EU1) ; DPF pour la maison mère américaine | Non vérifié | — | Registre DPF n° 5446 — VÉRIFIÉ ; hébergement EU1 — PROBABLE |
| **Twilio** (si utilisé pour la téléphonie) | Numéro et acheminement des appels | **Certifié, actif** (non RH) | DPF | — | — | Registre DPF n° 5394 — VÉRIFIÉ |
| **Deepgram** (transcription, si c'est le fournisseur configuré dans Vapi) | Reconnaissance vocale | **Non trouvé** | Non vérifié | Non vérifié | — | Registre DPF — VÉRIFIÉ (absence) ; fournisseur réellement configuré — À VÉRIFIER dans le compte Vapi |
| **Brevo** | Rappels e-mail/SMS | Sans objet (société française) | Traitement dans l'UE | — | — | Non vérifié aujourd'hui — PROBABLE |

## Ce que cela change

1. **Aucun transfert n'est sans base juridique** : chaque prestataire américain propose soit le DPF, soit des CCT.
   Pour Vapi, OpenAI, Airtable et probablement Deepgram, la base est **les CCT**, ce qui impose une
   **analyse d'impact des transferts (TIA)** documentée par AutomateLux.
2. **Mesure la plus efficace, gratuite** : activer le **Zero Data Retention de Vapi** et ne conserver les
   transcriptions que dans un stockage choisi par AutomateLux (idéalement dans l'UE). Cela réduit fortement
   ce qui reste aux États-Unis.
3. **Point de structure à trancher** : OpenAI et ElevenLabs sont-ils utilisés **avec les clés API
   d'AutomateLux** (sous-traitants directs : il faut accepter leurs DPA, OpenAI Ireland pour OpenAI) ou
   **via les clés de Vapi** (sous-traitants de Vapi, de second rang) ? L'annexe 1 doit le dire.
4. **Entraînement de l'IA** : vérifié uniquement pour l'API OpenAI (pas d'entraînement par défaut).
   À vérifier pour Vapi, ElevenLabs et Deepgram avant d'écrire une interdiction dans le contrat.

## À faire dans les comptes d'AutomateLux (impossible à vérifier de l'extérieur)

- Vapi : activer Zero Data Retention ; relever le fournisseur de transcription et la source des clés OpenAI / ElevenLabs.
- OpenAI : vérifier que le compte est rattaché à OpenAI Ireland Ltd et que le DPA est accepté.
- ElevenLabs et Airtable : vérifier que l'offre souscrite donne accès au DPA ; régler les options d'entraînement si elles existent.
- Conserver une copie datée de chaque DPA accepté.
