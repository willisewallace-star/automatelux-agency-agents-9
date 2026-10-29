# Vérification de SeaTable — 29/10/2026

| Point | Constat | Source | Confiance |
|---|---|---|---|
| Société | **SeaTable GmbH**, 117er Ehrenhof 5, 55118 Mayence, Allemagne, HRB 49723 (tribunal de Mayence), gérants Christoph et Dr Ralf Dyllick-Brenzinger | Mentions légales SeaTable | VÉRIFIÉ |
| **Développeur du logiciel** | **Seafile Ltd., Pékin, Chine** | Conditions d'utilisation et page « À propos » de SeaTable | VÉRIFIÉ |
| **Actionnariat** | Seafile détenait **50 %** de SeaTable GmbH à sa création | TechCrunch, 26/05/2023 | PROBABLE (situation actuelle non vérifiée) |
| Hébergement | **Exoscale** (Akenes SA, Lausanne, Suisse ; filiale du groupe A1 Telekom Austria), centres de données de **Francfort et Munich** | Page sécurité SeaTable (modifiée le 07/04/2026) | VÉRIFIÉ (déclaration du fournisseur) |
| Sauvegardes | Quotidiennes, dans un centre de données distant (en Europe) | Page sécurité | VÉRIFIÉ (déclaration) |
| Données hors UE | « Les données des utilisateurs ne quittent jamais l'Europe », **sauf les données d'abonnement et de paiement** | Page sécurité | VÉRIFIÉ (déclaration) |
| **Accès depuis la Chine** | « Dans des circonstances exceptionnelles (par ex. correction de bugs), des employés de **Seafile Ltd.** peuvent recevoir un accès à l'infrastructure de SeaTable Cloud », sous la supervision d'un employé de SeaTable GmbH | Page sécurité | VÉRIFIÉ |
| Contrat de sous-traitance (DPA) | **Public**, art. 28 RGPD, version allemande contraignante ; signature en ligne via un générateur | seatable.com/de/auftrag-zur-auftragsverarbeitung | VÉRIFIÉ |
| Clause de localisation | Art. 3.2 du DPA : traitement **exclusivement en Allemagne, dans l'UE ou l'EEE** ; **tout transfert vers un pays tiers exige l'accord préalable du client** | DPA SeaTable | VÉRIFIÉ |
| Liste des sous-traitants | Accessible **dans l'espace client** ou en annexe du DPA (pas sur une page publique) ; changement réputé accepté sans opposition sous 4 semaines | DPA, art. 7.2 | VÉRIFIÉ |
| Notification de violation | « Sans délai » (pas de délai chiffré) | DPA, art. 5.4 | VÉRIFIÉ |
| Certification | **Aucune** pour SeaTable ; centres de données Exoscale ISO 27001 ; test d'intrusion de septembre 2024 | Page sécurité | VÉRIFIÉ |
| Intégration Make.com | Application officielle sur Make | make.com/integrations/seatable | VÉRIFIÉ |
| Prix | Plus : **7 €/utilisateur/mois** (annuel), 50 000 lignes, **10 000 appels API par utilisateur et par mois** ; Enterprise : 14 € | Page tarifs SeaTable | VÉRIFIÉ |

## Analyse

- **Point fort** : le contrat de sous-traitance est public et l'art. 3.2 **interdit tout transfert hors UE/EEE
  sans l'accord préalable du client**. C'est contractuellement plus protecteur que tout ce que Baserow publie.
- **Point faible majeur** : le logiciel est développé par une société de **Pékin**, qui peut recevoir un accès
  exceptionnel aux serveurs, et qui détenait la moitié du capital en 2023. Un accès à distance depuis la Chine
  constitue un **transfert vers un pays sans décision d'adéquation**. La loi chinoise sur le renseignement
  national (art. 7) impose aux organisations de coopérer avec les services de renseignement **[PROBABLE — à
  faire confirmer par un juriste]**.
- **Contradiction à éclaircir** : la page sécurité prévoit l'accès de Seafile ; le DPA exige l'accord préalable
  du client pour tout transfert hors EEE. On ne sait pas si SeaTable demande cet accord avant un accès de Seafile.
- L'évaluation tierce « EU-Sovereign » (EU Vetted) **ne mentionne pas** ce lien avec la Chine : elle est incomplète.

## Questions à envoyer à SeaTable

1. Seafile Ltd. (Pékin) détient-elle encore une participation dans SeaTable GmbH, et de quel pourcentage ?
2. Un accès de Seafile Ltd. à SeaTable Cloud est-il traité comme un transfert soumis à l'accord préalable du
   client (art. 3.2 du DPA) ? Peut-on refuser tout accès de Seafile aux données d'AutomateLux ?
3. Combien d'accès de Seafile ont eu lieu sur les 12 derniers mois ? Sont-ils journalisés et communiqués ?
4. Merci de nous transmettre la liste à jour des sous-traitants.
