# Voice-pack-Proscenic-M6-pro

Ce projet propose des packs audio personnalisés pour l'aspirateur **Proscenic M6 Pro**.

> ⚠️ Il est possible de changer les audios sans Valetudo, mais **il est fortement recommandé de l'utiliser**.

## 🔧 Prérequis

Suivez **au moins** la partie *connexion au shell* de ce guide :  
👉 [https://github.com/Hypfer/valetudo-crl200s-root](https://github.com/Hypfer/valetudo-crl200s-root)

---

## 💾 Sauvegarder les audios d'origine

```
adb pull /usr/share/audio/english/ export
```
❌ Supprimer le pack actuel
```
adb shell
```
```
rm -r /usr/share/audio/english/
```
📦 Installer un nouveau pack

Clonez ce dépôt :
```
git clone https://github.com/95P10Aa4Ob/Voice-pack-Proscenic-M6-pro.git
```
Choisissez un pack :

    english_sauv — pack d'origine

    francais_normal — voix française classique

    francais_humour — voix française avec humour

Renommez le dossier choisi en english.

Poussez le nouveau pack sur l'appareil :
```
    adb push english /usr/share/audio/english
```
