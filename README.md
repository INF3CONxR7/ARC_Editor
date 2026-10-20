<p align="center">
  <img src="logo.png" alt="Logo d’ARC Editor" width="128">
</p>

<h1 align="center">ARC Editor</h1>

<p align="center">
  Explorez et modifiez les archives <b>.arc</b> de <b>Minecraft PlayStation 3 Edition</b> (MediaPS3.arc, media.arc des
  packs) :<br>aperçu des images et des interfaces <b>.fui</b>, remplacement, export, ajout et renommage des fichiers.
</p>

<p align="center">
  <a href="https://github.com/INF3CONxR7/ARC_Editor/releases/latest"><img src="https://img.shields.io/github/v/release/INF3CONxR7/ARC_Editor?label=t%C3%A9l%C3%A9charger&color=28C860" alt="Télécharger"></a>
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011-0078D6?logo=windows&logoColor=white" alt="Windows 10 et 11">
  <a href="https://discord.gg/TbFYvqsh5z"><img src="https://img.shields.io/badge/Discord-rejoindre-5865F2?logo=discord&logoColor=white" alt="Serveur Discord"></a>
</p>

---

## Sommaire

- [Fonctionnalités](#fonctionnalités)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Raccourcis clavier](#raccourcis-clavier)
- [Mises à jour et Discord](#mises-à-jour-et-discord)
- [En cas de problème](#en-cas-de-problème)
- [Désinstaller](#désinstaller)
- [Crédits](#crédits)
- [Support](#support)
- [English](#english)

## Fonctionnalités

- **Ouverture des archives .arc** de Minecraft PS3 (`USRDIR\Common\Media\MediaPS3.arc`, `media.arc` des packs de
  textures et des mash-ups), par le menu, un glisser-déposer ou un double-clic sur le fichier.
- **Liste des fichiers** avec dossiers repliables (Graphics, Structures…), tri naturel, recherche instantanée et
  filtres (images, interfaces, autres).
- **Aperçu** : images PNG et JPEG avec zoom, déplacement et damier de transparence (pixels nets pour les textures),
  **images intégrées aux interfaces .fui** (bande de vignettes), tables de couleurs `.col`, textes, et aperçu
  hexadécimal pour le reste. Un dossier choisi s’affiche en **galerie**.
- **Remplacement** d’un fichier ou d’une image d’interface : les images sont converties en PNG 32 bits (le format du
  jeu), et une résolution différente de l’originale est signalée avant.
- **Export** d’un fichier, d’un dossier, de toutes les images d’une interface ou de l’archive entière.
- **Éditeur de langues** : un double-clic sur `languages.loc` ouvre les textes du jeu, langue par langue (21 langues,
  plus de 4 600 textes), avec recherche ; les traductions modifiées retournent dans l’archive. Un fichier `.loc` du
  disque s’ouvre aussi seul (*Ouvrir avec*).
- **Ajout, renommage, suppression et restauration** des fichiers, avant enregistrement.
- **Enregistrement sûr** : l’archive est écrite à côté puis mise à la place (jamais à moitié écrite), et une copie de
  l’original (`.bak`) est gardée au premier enregistrement. L’ordre des fichiers d’origine est conservé.
- **Mises à jour automatiques** et **présence Discord**.

## Installation

1. Ouvrez la [dernière version](https://github.com/INF3CONxR7/ARC_Editor/releases/latest) et téléchargez
   **`ARCEditor-win-x64.zip`** (le fichier `.zip.sig` sert au programme de mise à jour : inutile de le télécharger).
2. Extrayez l’archive à l’endroit de votre choix, par exemple dans Documents ou sur le Bureau : vous obtenez le dossier
   **`ARCEditor-win-x64`**. Gardez ensemble les deux fichiers qu’il contient.
3. Lancez **`ARC Editor.exe`** depuis ce dossier.

Il faut un PC sous **Windows 10 ou 11 (64 bits)**. Rien d’autre à installer : le runtime .NET est inclus dans
l’exécutable.

> **Windows SmartScreen** : l’exécutable n’est pas signé Authenticode, Windows peut donc afficher « Windows a protégé
> votre ordinateur ». Cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**.

## Utilisation

1. **Ouvrir** : *Fichier > Ouvrir une archive*, ou glissez un `.arc` dans la fenêtre. Travaillez sur une copie de la
   backup, ou gardez la case *Garder une copie de l’original (.bak)* cochée.
2. **Trouver un fichier** : dans la liste, ou par la recherche en haut à droite (`Ctrl+F`).
3. **Remplacer** : bouton *Remplacer* (ou glissez une image sur l’aperçu). Dans une interface `.fui`, c’est l’image
   choisie dans la bande de vignettes qui est remplacée.
4. **Enregistrer** : `Ctrl+S`. Les fichiers changés sont marqués d’un point (ambre : modifié, vert : ajouté), et la
   ligne d’état indique le nombre de modifications à enregistrer.
5. **Sur la PS3** : remettez l’archive à sa place dans le jeu (par exemple
   `/dev_hdd0/game/NPEB01899/USRDIR/Common/Media/MediaPS3.arc`).

Conseils : gardez la **même résolution** que l’image d’origine (ou un multiple pour un pack HD), et ne renommez pas
les fichiers d’origine : le jeu les cherche par leur nom.

## Raccourcis clavier

| Touche | Action |
|---|---|
| `Ctrl+O` / `Ctrl+S` / `Ctrl+Maj+S` | Ouvrir / Enregistrer / Enregistrer sous |
| `Ctrl+F` | Rechercher |
| `Ctrl+R` / `Ctrl+E` | Remplacer / Exporter l’élément choisi |
| `F2` / `Suppr` | Renommer / Supprimer (dans la liste) |
| `Ctrl++` / `Ctrl+-` / `Ctrl+0` / `Ctrl+1` | Zoom avant / arrière / ajusté / taille réelle (la molette zoome aussi) |
| `F11` / `Échap` | Agrandir l’aperçu / revenir |

## Mises à jour et Discord

- **Mises à jour** : au démarrage, l’application vérifie sur GitHub si une nouvelle version est publiée. Si c’est le
  cas, **« Mise à jour X.Y.Z disponible »** apparaît en haut à droite : un clic, et l’application se ferme (après vous
  avoir proposé d’enregistrer l’archive), installe la mise à jour, puis se relance. Chaque version est **signée** :
  une version dont la signature est absente ou invalide est refusée.
- **Présence Discord** : si Discord est ouvert, votre profil indique ce que fait l’application (parcourt, modifie,
  enregistre une archive), jamais le nom de vos fichiers. Le bouton aux ondes, à côté de la version, l’affiche ou la
  masque.
- Les logos Discord et GitHub de l’en-tête ouvrent le serveur Discord et la page GitHub de l’auteur.

## En cas de problème

| Problème | Solution |
|---|---|
| « Archive illisible » | Le fichier n’est pas une archive `.arc` de Minecraft PS3, ou il est tronqué : reprenez-le dans la backup. |
| Le jeu affiche mal une image remplacée | Gardez la résolution d’origine et un PNG classique (l’application convertit les autres formats). |
| Le double-clic n’ouvre pas les `.arc` | Un autre programme les ouvre déjà : clic droit, *Ouvrir avec*, puis ARC Editor. |
| L’enregistrement échoue | Le dossier est peut-être en lecture seule ou l’archive ouverte ailleurs : *Enregistrer sous* dans un autre dossier. L’archive d’origine reste intacte. |

Une question ? Rejoignez le [serveur Discord](https://discord.gg/TbFYvqsh5z).

## Désinstaller

Supprimez le dossier de l’application. Elle garde aussi, pour votre compte Windows :

| Emplacement | Contenu |
|---|---|
| `HKEY_CURRENT_USER\Software\ARCEditor` | Réglages (dossiers, affichage, archives récentes, activité Discord). |
| `HKEY_CURRENT_USER\Software\Classes\.arc` et `…\ARCEditor.Archive` | Ouverture des `.arc` par double-clic. |
| `%LocalAppData%\ARC Editor` | Journal des mises à jour. |

Vous pouvez supprimer ces clés et ce dossier.

## Crédits

- **ARC Editor** : © 2026 INF3C7ONxR7. Tous droits réservés.
- **Format des archives** : d’après MUArchiveEditor et la bibliothèque OMI (PhoenixARC et la communauté Minecraft
  Legacy Console Edition).
- **Logos Discord et GitHub** : tracés de [Simple Icons](https://simpleicons.org/) (CC0) ; ces logos sont des marques
  de leurs propriétaires.

Projet non officiel, sans lien avec Mojang, Microsoft, 4J Studios ni Sony. Minecraft est une marque de Mojang ;
PlayStation et PS3 sont des marques de Sony Interactive Entertainment.

## Support

- Discord : [discord.gg/TbFYvqsh5z](https://discord.gg/TbFYvqsh5z)
- Soutenir le projet : [ko-fi.com/INF3C7ONxR7](https://ko-fi.com/INF3C7ONxR7)

Développé par **INF3C7ONxR7**.

---

## English

**ARC Editor** browses and edits the **.arc** archives of **Minecraft PlayStation 3 Edition** (MediaPS3.arc, pack
media.arc files). The interface is in French.

**Requirements**: Windows 10 or 11 (64-bit) PC, nothing else to install (the .NET runtime is included).

**Features**: folder tree, natural sort, instant search and filters · preview of PNG/JPEG images (zoom, pan,
transparency checkerboard, crisp pixels), of the images embedded in **.fui** interfaces, of `.col` color tables, texts
and a hex view · folder gallery · replace a file or an interface image (converted to 32-bit PNG, resolution changes
flagged) · export a file, a folder, all images of an interface or the whole archive · add, rename, delete and restore
files · safe saving (written next to the archive, then swapped in; original kept as `.bak`) · automatic updates and
Discord presence.

**Install**: download **`ARCEditor-win-x64.zip`** from the
[latest release](https://github.com/INF3CONxR7/ARC_Editor/releases/latest) (not the `.sig` file, used by the
updater), extract it to get the **`ARCEditor-win-x64`** folder and run **`ARC Editor.exe`**. The executable is not
Authenticode-signed, so Windows SmartScreen may show "Windows protected your PC": click **More info**, then **Run
anyway**.

**Uninstall**: delete the app folder. Settings are in `HKEY_CURRENT_USER\Software\ARCEditor`, the `.arc` file
association in `HKEY_CURRENT_USER\Software\Classes\.arc` and `…\ARCEditor.Archive`, the update log in
`%LocalAppData%\ARC Editor`.

Unofficial project, not affiliated with Mojang, Microsoft, 4J Studios or Sony.

**Support**: [Discord](https://discord.gg/TbFYvqsh5z) · [Ko-fi](https://ko-fi.com/INF3C7ONxR7) · Developed by
**INF3C7ONxR7**.
