# Tourniquet — La Famille Parfaite

**L'application Windows de [lolesport.lafamilleparfaite.com](https://lolesport.lafamilleparfaite.com), la communauté québécoise de League of Legends.**  
Cups du samedi, équipes, organisations, tournois, scrims, billets, statistiques et Généa-LoL, dans une application rapide, en français et en anglais, qui se met à jour toute seule.

> **Version 1.0** · Windows 10 et 11 · *English summary at the bottom.*

---

## Télécharger

👉 **[lolesport.lafamilleparfaite.com/telecharger](https://lolesport.lafamilleparfaite.com/telecharger)**

| Fichier | C'est quoi |
|---|---|
| `LoLEsport-win-Setup.exe` | **L'installateur.** Double-clic : Tourniquet s'installe dans ton dossier Windows (aucun droit d'administrateur), crée son raccourci et se met à jour tout seul. |
| `LoLEsport-win-Portable.zip` | **La version portable.** Décompresse le dossier n'importe où et lance `LolEsport.exe` : rien n'est installé. |

Windows peut afficher « Windows a protégé votre ordinateur » : l'application n'est pas encore signée par un certificat payant. Clique **Informations complémentaires → Exécuter quand même**, après avoir vérifié l'empreinte du fichier (ci-dessous).

---

## ⚠️ Bug connu – Fiche de joueur

Un problème technique dans l'application empêche actuellement de compléter la fiche de joueur directement depuis l'application et de faire passer l'étape au vert.

En attendant la publication d'un correctif, **vous pouvez compléter votre fiche directement sur le site web**. La synchronisation avec l'application se fera automatiquement. 

*(Note : La fonction des champions détestés nécessite un forfait payant).*

👉 **Remplir votre fiche sur le site :** [https://lolesport.lafamilleparfaite.com/tableau?tab=fiche](https://lolesport.lafamilleparfaite.com/tableau?tab=fiche)

Désolé pour cet inconvénient et merci pour votre patience pendant que nous travaillons sur le correctif !

---

## ⚠️ Known Bug – Player Card

A technical issue currently prevents completing the player card step directly within the app (turning it green).

While we work on a fix, **you can complete your player card directly on the website**. It will sync properly with the app.

*(Note: The hated champions feature requires a paid plan).*

👉 **Complete your card on the website:** [https://lolesport.lafamilleparfaite.com/tableau?tab=fiche](https://lolesport.lafamilleparfaite.com/tableau?tab=fiche)

We apologize for the inconvenience and thank you for your patience!

---

## Ce que fait Tourniquet

| | |
|---|---|
| 🏆 **Les Cups du samedi** | Vote de la Cup, plage horaire, tableau, sélection des champions, code de partie, résultats, palmarès |
| 🛡️ **Équipes et organisations** | Créer, inviter, gérer, annonces, page de présentation, tournois d'organisation (droit d'inscription et prix en argent, conditions et règlement) |
| ⚔️ **Scrims et Lobby** | Offres de scrims, listes d'amis, joueurs du Québec |
| 📊 **Statistiques** | Parties, notes de match, partenaires, analyse des matchs de Cup |
| 🎟️ **La bourse et la boutique** | Billets, jetons, Forfait Parfait, chandails et merch (paiement sur la page sécurisée de Stripe) |
| 🌳 **Généa-LoL** | L'arbre des liens entre joueurs |
| 🔄 **Mises à jour automatiques** | La nouvelle version se télécharge, puis propose « Redémarrer maintenant / Plus tard » |

Tourniquet fonctionne aussi sur un PC sans League of Legends installé, à l'exception des fonctionnalités qui communiquent directement avec le client du jeu (ex. importer sa liste d'amis, ouvrir une partie personnalisée).

---

## Vérifier un fichier téléchargé (SHA-256)

La page de téléchargement affiche l'empreinte SHA-256 de chaque fichier. Dans PowerShell, dans le dossier du téléchargement :

```powershell
Get-FileHash .\LoLEsport-win-Setup.exe -Algorithm SHA256
```

Le résultat doit être identique à l'empreinte affichée sur la page. Un seul octet changé donne une empreinte complètement différente.

## Sécurité

- **Aucune clé dans l'application** : ni Riot, ni Discord, ni Stripe. Elles restent sur le serveur, qui revérifie chaque action.
- **Paiements** : Tourniquet ouvre seulement les pages sécurisées de Stripe. Il ne voit jamais ta carte. Les organisations reçoivent l'argent de leurs tournois sur leur propre compte Stripe, sans jamais donner de clé.
- **Ta connexion** est gardée chiffrée sur ton PC (protection de Windows).
- **Ton compte Riot** : son identifiant technique (PUUID) n'est jamais affiché ni envoyé à d'autres joueurs.
- **Chaque version officielle a une empreinte** connue du serveur : une copie modifiée est repérée.

Un problème de sécurité ? Écris à **support@lafamilleparfaite.com** avant d'en parler publiquement.

## Signaler un bogue

Le bouton **« 🐞 Trouver un bug »**, en bas de chaque page de l'application, ou **support@lafamilleparfaite.com**.

## Droits

- © 2026 La Famille Parfaite. **Tous droits réservés** — voir [LICENCE.txt](LICENCE.txt).
- **League of Legends** : *Tourniquet — La Famille Parfaite isn't endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing League of Legends. League of Legends and Riot Games are trademarks or registered trademarks of Riot Games, Inc.*

---

## English summary

**Tourniquet** is the Windows app of [lolesport.lafamilleparfaite.com](https://lolesport.lafamilleparfaite.com), the Quebec League of Legends community: Saturday Cups, teams, organizations, tournaments, scrims, tickets, stats and Généa-LoL, in French and English, with automatic updates.

- **Download**: [lolesport.lafamilleparfaite.com/telecharger](https://lolesport.lafamilleparfaite.com/telecharger) — `LoLEsport-win-Setup.exe` (installer, automatic updates) or `LoLEsport-win-Portable.zip` (unzip and run `LolEsport.exe`). Works without League of Legends installed, except features that talk to the local game client.
- **Verify your download**: `Get-FileHash .\LoLEsport-win-Setup.exe -Algorithm SHA256` must match the fingerprint shown on the download page.
- **Security**: no keys in the app, payments only on Stripe's secure pages, Riot PUUIDs never shown. Report security issues to support@lafamilleparfaite.com.
- © 2026 La Famille Parfaite — **all rights reserved**. See [LICENCE.txt](LICENCE.txt).
