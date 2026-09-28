# Politique de confidentialité — MyFridge

> **Brouillon de travail, pas un document validé juridiquement.** Basé sur les données réellement collectées dans le code au 2026-08-28 (voir « Périmètre » ci-dessous). Les champs entre crochets `[À COMPLÉTER]` doivent être remplis avant publication. À faire relire par un professionnel avant mise en ligne, notamment les sections Responsable du traitement, Transferts hors UE et Mineurs.

*Dernière mise à jour : 28 septembre 2026*

## 1. Qui sommes-nous

MyFridge est une application mobile de gestion de frigo anti-gaspillage, éditée par Axel Paupier, auto-entrepreneur (SIRET 109 301 820 00014).

**Responsable du traitement :** Axel Paupier (auto-entrepreneur)
**Contact pour toute question relative à vos données :** my.fridge.antiwaste@gmail.com

## 2. Données que nous collectons

Uniquement les données nécessaires au fonctionnement de l'application :

| Donnée | Pourquoi | Où elle est stockée |
|---|---|---|
| E-mail (compte) | Créer et sécuriser ton compte, te reconnecter | Supabase (authentification) |
| Contenu de ton frigo (noms d'aliments, code-barres scannés, catégories, quantités, dates de péremption, photos produit) | Faire fonctionner l'app (suivi du frigo, alertes de péremption, suggestions de recettes) | Supabase (base de données), lié à ton compte |
| Liste de courses | Faire fonctionner la liste de courses | Supabase |
| Historique « utilisé / jeté » | Calculer ton impact anti-gaspillage (aliments sauvés) | Supabase |
| Points de jeu (Glaçons 🧊 / FrigoCoins 💎) et mouvements associés | Gamification, achats dans la boutique | Supabase |
| Langue et skin de frigo choisis | Personnalisation de l'affichage | Uniquement sur ton téléphone (stockage local), jamais envoyé à nos serveurs |
| Progression des étapes de recette cochées | Reprendre une recette là où tu l'as laissée | Uniquement sur ton téléphone (stockage local) |
| Autorisation caméra | Scanner les codes-barres (le flux vidéo n'est jamais enregistré ni transmis) | Traité localement sur ton téléphone |
| Autorisation notifications | T'envoyer un rappel quotidien si des aliments périment bientôt | Notifications programmées localement sur ton téléphone, aucune donnée envoyée à un serveur pour ça actuellement |
| Données d'usage (écrans consultés, actions comme « produit ajouté », « recette terminée », « scan »), associées à ton e-mail si tu es connecté | Mesurer l'usage réel de l'app pour l'améliorer (quelles fonctionnalités sont utiles, où les gens bloquent) | PostHog (hébergé en Union européenne) |

**Ce que nous ne collectons PAS (à date) :** pas de données de localisation, pas de données de paiement (gérées directement par Apple/Google), pas de suivi de plantage (Sentry — pas encore actif dans l'app), pas de publicité.

> Cette liste évoluera avec l'app (Sentry et de la publicité sont prévus dans la roadmap) — cette politique devra être mise à jour à ce moment-là, et un bandeau de consentement ajouté le cas échéant.

## 3. Pourquoi on traite ces données (base légale RGPD)

- **Exécution du contrat** (article 6.1.b) : la quasi-totalité des données ci-dessus sont nécessaires pour te fournir le service que tu utilises (gérer ton frigo, tes recettes, ta liste de courses).
- **Intérêt légitime** (article 6.1.f) : mesure de ton impact anti-gaspillage, personnalisation, mesure d'usage via PostHog pour améliorer l'app. [À COMPLÉTER avant publication : faire confirmer par un professionnel si l'intérêt légitime suffit pour PostHog ou si un consentement explicite (bandeau) est requis — PostHog associe les événements à ton e-mail, ce n'est pas un tracking strictement anonyme.]
- **Consentement** (article 6.1.a) : autorisations caméra et notifications, demandées explicitement par le système d'exploitation et révocables à tout moment dans les réglages de ton téléphone.

## 4. Avec qui tes données sont partagées

- **Supabase** (hébergement, base de données, authentification) — sous-traitant technique, données hébergées en France (région du projet Supabase). Voir la politique de confidentialité et le DPA de Supabase : https://supabase.com/privacy
- **Open Food Facts** — quand tu scannes un code-barres, ce code (pas de donnée personnelle) est envoyé à l'API publique Open Food Facts pour récupérer les informations du produit. Voir leur politique : https://world.openfoodfacts.org/privacy
- **PostHog** (mesure d'usage) — sous-traitant technique, données hébergées en Union européenne. Voir leur politique : https://posthog.com/privacy
- Nous ne vendons ni ne louons tes données à personne.
- Tes données restent hébergées au sein de l'Union européenne (France) : à ce jour, aucun transfert hors UE.

## 5. Combien de temps on les garde

Tant que ton compte existe. Si tu supprimes ton compte, tes données sont supprimées **immédiatement** de notre base (suppression en cascade dès que le compte d'authentification est supprimé).

## 6. Tes droits

Conformément au RGPD, tu peux à tout moment :
- **Accéder** à tes données et en demander une **copie** (portabilité)
- Les faire **rectifier** si elles sont inexactes
- Demander leur **suppression**
- T'**opposer** à un traitement ou en demander la **limitation**

Pour exercer ces droits : écris-nous à my.fridge.antiwaste@gmail.com, ou utilise directement le bouton « Supprimer mon compte » dans Paramètres → Compte pour la suppression. Tu peux aussi introduire une réclamation auprès de la CNIL (www.cnil.fr) si tu penses que tes droits ne sont pas respectés.

## 7. Sécurité

Tes données sont protégées par un système d'accès strict (Row Level Security Supabase) : chaque utilisateur ne peut voir et modifier que ses propres données, jamais celles d'un autre. Les échanges entre l'app et nos serveurs sont chiffrés (HTTPS).

## 8. Mineurs

MyFridge est accessible à tout public. En France, la création d'un compte par un mineur de moins de 15 ans nécessite le consentement d'un titulaire de l'autorité parentale (article 8 du RGPD tel que transposé en droit français) ; ce seuil varie selon le pays de résidence au sein de l'Union européenne (de 13 à 16 ans).

[À COMPLÉTER avant la V2 boutique — le mécanisme de recueil de ce consentement parental n'est pas encore implémenté techniquement, et la boutique (achats réels, « boîte mystère ») nécessitera une vigilance renforcée pour les comptes mineurs : voir la note sur la réglementation des loot boxes évoquée précédemment.]

## 9. Modifications de cette politique

Cette politique peut évoluer, notamment à l'ajout de nouvelles fonctionnalités (analytics, publicité). Toute modification substantielle te sera signalée dans l'app.
