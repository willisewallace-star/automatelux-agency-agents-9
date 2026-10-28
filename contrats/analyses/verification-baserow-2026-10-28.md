# Vérification de Baserow — 28/10/2026

| Point | Constat | Source | Confiance |
|---|---|---|---|
| Société | **Baserow B.V.**, Keurenplein 4, Amsterdam, Pays-Bas, Chambre de commerce n° 81129254 | Conditions générales Baserow, art. 1.1 | VÉRIFIÉ |
| Actionnariat | Contrôle européen, pas de maison mère américaine identifiée | EU Vetted (évaluation tierce) | PROBABLE |
| Lieu de stockage | « Toutes les données clients de Baserow Cloud sont stockées exclusivement en Allemagne » | Blog officiel Baserow, 07/04/2026 | VÉRIFIÉ (déclaration du fournisseur) |
| Hébergeur en Allemagne | **Non publié.** Le site de Baserow sert ses propres fichiers depuis Amazon S3 : indice, pas preuve | Observation directe ; EU Vetted | NON VÉRIFIABLE |
| Contrat de sous-traitance (DPA) | **Mentionné dans les conditions générales (art. 12.2) mais non publié** ; la page /dpa n'existe pas | Conditions générales ; test direct | VÉRIFIÉ |
| Liste des sous-traitants | **Non publiée** | EU Vetted ; recherche directe | VÉRIFIÉ (absence) |
| Droit applicable | Droit néerlandais, tribunaux d'Amsterdam | Conditions générales, art. 15 | VÉRIFIÉ |
| Plafond de responsabilité de Baserow | Sommes payées sur les 12 derniers mois | Conditions générales, art. 10.2 | VÉRIFIÉ |
| Clause à clarifier | Art. 8.4 : Baserow peut exploiter « sans restriction » les informations dont il prend connaissance pendant le contrat. Vise a priori des éléments techniques, mais la rédaction est large | Conditions générales, art. 8.4 | À FAIRE CONFIRMER par le DPA |
| Intégration Make.com | Module officiel : surveiller les nouvelles lignes, créer, lire, modifier, supprimer une ligne, appel API | Documentation Baserow et page Make | VÉRIFIÉ |
| Prix (cloud) | Gratuit : 3 000 lignes ; Premium : 10 $/utilisateur/mois (annuel), 50 000 lignes ; Advanced : 18 $, 250 000 lignes. Prix en dollars | Page tarifs et documentation Baserow | VÉRIFIÉ |
| Sécurité annoncée | SOC 2 Type II, chiffrement au repos et en transit, sauvegardes | Blog officiel | Déclaration du fournisseur |

## Conclusion

Baserow est **européen et stocke les données en Allemagne**, mais **ni son contrat de sous-traitance ni
la liste de ses sous-traitants ne sont publics**. Sans ces deux documents, AutomateLux ne peut pas
remplir honnêtement l'annexe 1 de son propre contrat (hébergeur, sous-traitants, absence de transfert).

## Alternative identifiée : SeaTable

SeaTable GmbH (Mayence, Allemagne), hébergement en Allemagne (Exoscale et Hetzner), **contrat de
sous-traitance et liste des sous-traitants publics**, intégration Make.com officielle, à partir de
7 €/utilisateur/mois. **Source : comparatifs et évaluations tiers (EU Vetted, SeaTable) — non vérifié
directement auprès des documents de SeaTable.**

## Questions à envoyer à Baserow si on le garde

1. Merci de nous transmettre votre Data Processing Agreement (art. 12.2 de vos conditions).
2. Quel est l'hébergeur de Baserow Cloud en Allemagne, et quelle est la liste complète de vos sous-traitants ?
3. Des données (sauvegardes, journaux, support, e-mails) sont-elles traitées hors de l'UE ?
4. L'article 8.4 de vos conditions peut-il viser les données stockées par vos clients ?
