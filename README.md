# Budget

Application de budget personnelle, **privée par conception** :

- Aucune donnée ne quitte l'appareil : pas de serveur, pas de tracking, aucune connexion externe (CSP stricte).
- Données chiffrées en AES-256-GCM avec une clé dérivée du mot de passe (PBKDF2-SHA256, 310 000 itérations).
- Import CSV des relevés bancaires (KBC, BNP Paribas Fortis, ING, Belfius… détection automatique des colonnes).
- Anti-doublons : référence bancaire ou empreinte date + montant + libellé, gestion des chevauchements et des doublons légitimes.
- IBAN, numéros de carte et communications structurées masqués à l'import.
- Sauvegarde chiffrée et synchronisation entre appareils par fichier.

⚠️ Ne jamais committer de relevé bancaire ou de sauvegarde dans ce dépôt.
