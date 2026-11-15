# Glose pour macOS

Glose est une languette au bord de l'écran : on la touche, le panneau de notes s'ouvre. Les notes se rangent
automatiquement, une recherche porte sur tout, et une relecture par Haiku (Claude) propose des corrections en
montrant l'avant et l'après. Des dossiers intelligents proposent une place à chaque note, et un serveur MCP
permet à Claude Code d'utiliser les notes.

Ce dépôt ne contient que les versions à installer. Le code source n'est pas public.

## Ce qu'il faut

- un Mac à puce Apple (M1 ou plus récent) ;
- macOS 15 ou plus (le verre « Liquid Glass » sous macOS 26, un fond translucide du système en dessous).

## Installer

Dans Terminal (Cmd + Espace, « Terminal »), une seule commande, qui installe aussi les mises à jour :

```
curl -fsSL https://raw.githubusercontent.com/LucasHRCHatReply/glose-releases/main/installer.sh | zsh
```

Le script télécharge la dernière version, vérifie l'empreinte SHA-256 du zip, l'identifiant de l'app et sa signature
(équipe Apple `JT9FY7PP7K`, `codesign --verify --deep --strict`), copie l'app dans ~/Applications, puis l'ouvre.
