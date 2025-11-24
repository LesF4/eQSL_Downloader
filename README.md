# eQSL_Downloader
eQSL_Downloader is an application that allows you to download QSL cards available on eQSL.
Développé par **F4LPS** avec l'aide de **F4LCL** - 73 📻

---

## 🚀 Démarrage rapide

1. **Double-cliquez** sur `eQSL_Downloader.exe`
2. **Choisissez votre langue** en haut à droite
3. **Entrez vos identifiants** eQSL.cc
4. **Configurez vos options** et cliquez sur "Démarrer"
5. **Vos QSL** sont téléchargées et organisées automatiquement !

> ⚠️ **Première utilisation** : Le démarrage peut prendre 10-20 secondes (c'est normal)

---

## ✨ Fonctionnalités

✅ **6 langues** : Français, English, Deutsch, Italiano, Português, Español  
✅ **200+ pays DXCC** reconnus automatiquement  
✅ **Organisation automatique** par pays dans des dossiers  
✅ **Détection des doublons** - évite les téléchargements multiples  
✅ **Filtres avancés** : Inbox, Archives, dates, pays  
✅ **Statistiques en temps réel**  
✅ **Rapport détaillé** des QSL ignorées  

---

## 📋 Avant de commencer

**Vous avez besoin de :**
- ✅ Un compte actif sur **eQSL.cc**
- ✅ Votre **Indicatif** (callsign)
- ✅ Votre **Mot de passe** eQSL
- ✅ Votre **QTH Nickname** (trouvez-le sur eQSL.cc → My Profile)
- ✅ Une **connexion Internet**

---

## 🖥️ Utilisation

### 1️⃣ Identifiants

Remplissez vos informations eQSL :
- **Indicatif** : Votre callsign (ex: F4LPS)
- **Mot de passe** : Votre mot de passe eQSL.cc
- **QTH Nickname** : Visible dans votre profil eQSL
- ☑️ **Cochez** "Enregistrer les identifiants" pour ne plus les ressaisir

### 2️⃣ Options de téléchargement

**📥 INBOX (Boîte de réception)**
- ✅ Inclure confirmées
- ❓ Inclure non confirmées

**🗄️ ARCHIVES**
- ✅ Inclure confirmées
- ❓ Inclure non confirmées

> 💡 **Astuce** : Par défaut, seule l'Inbox est cochée. Cochez les Archives pour tout télécharger.

**🌍 Filtrer par pays**
- Choisissez un pays spécifique
- Ou laissez "Tous les pays" pour une organisation automatique

**📅 Période**
- Date début : AAAAMMJJ (ex: 20240101)
- Date fin : AAAAMMJJ (ex: 20241231)

**📁 Dossier destination**
- Par défaut : `QSL_Cards` à côté du programme
- Cliquez sur "Parcourir" pour choisir un autre dossier

### 3️⃣ Téléchargement

1. Cliquez sur **🚀 DÉMARRER LE TÉLÉCHARGEMENT**
2. Suivez la progression en temps réel
3. Les statistiques s'actualisent automatiquement
4. Cliquez sur **⏹️ ARRÊTER** pour interrompre

### 4️⃣ Résultats

Vos QSL sont organisées dans des dossiers par pays :

```
QSL_Cards/
├── France/
├── France-TM/          (Stations temporaires TM)
├── Allemagne/
├── USA/
├── Japon/
├── Autres/
├── .qsl_cache.json    (NE PAS SUPPRIMER - évite les doublons)
└── qsl_ignorees.txt   (Rapport détaillé)
```

**Format des fichiers** : `INDICATIF_DATE_HEURE_BANDE_MODE.jpg`

**Exemple** : `F4ABC_20241115_1430_20M_SSB.jpg`

---

## ⚠️ Avertissement Antivirus

### C'est normal !

Votre antivirus peut afficher une alerte de type :
- "Fichier non reconnu"
- "Éditeur inconnu"
- "Menace potentielle"

**C'est un FAUX POSITIF** très courant avec les programmes Python compilés.

### Pourquoi ?

Les exécutables créés avec PyInstaller sont souvent signalés par les antivirus car :
- Le programme n'a pas de signature numérique payante (~300€/an)
- Les antivirus sont prudents avec les nouveaux fichiers
- C'est une protection normale

### Que faire ?

**Option 1** : Ajouter une exception dans votre antivirus
1. Ouvrez votre antivirus (Windows Defender, Avast, etc.)
2. Ajoutez `eQSL_Downloader.exe` aux exceptions/exclusions
3. Relancez le programme

**Option 2** : Analyser le fichier en ligne
- VirusTotal : https://www.virustotal.com
- Uploadez le fichier pour une analyse multi-antivirus
- Vous verrez que la majorité le reconnaît comme sûr

**Option 3** : Utiliser le code source
- Téléchargez le code source Python
- Lancez avec `python eqsl_downloader_gui.py`
- Contact : developpement@lesf4.fr

### 🔒 Sécurité garantie

✅ **Code open source** : Transparence totale  
✅ **Aucune collecte de données**  
✅ **Aucune transmission à des tiers**  
✅ **Connexion HTTPS sécurisée** avec eQSL.cc  
✅ **Testé par F4LCL** et la communauté radioamateur  

---

## ❓ Problèmes courants

### Le programme ne démarre pas
- ⏳ **Première utilisation** : Patientez 10-20 secondes
- 🛡️ **Antivirus** : Ajoutez une exception
- 🔄 **Redémarrage** : Fermez et relancez

### Erreur d'authentification
- ✅ Vérifiez votre indicatif
- ✅ Vérifiez votre mot de passe
- ✅ Vérifiez votre QTH Nickname sur eQSL.cc
- ✅ Testez votre connexion sur le site eQSL.cc

### Erreur "Accès refusé" au dossier
- 📁 Choisissez un autre dossier de destination
- 🔓 Vérifiez les permissions d'écriture
- 👮 Lancez en tant qu'administrateur (clic droit sur l'exe)

### Aucune QSL trouvée
- ✅ Vérifiez que vous avez des QSL sur eQSL.cc
- ✅ Vérifiez au moins une option est cochée (Inbox ou Archive)
- ✅ Vérifiez vos filtres de dates
- ✅ Essayez sans filtre de pays

### Les QSL sont téléchargées en double
- ⚠️ **NE SUPPRIMEZ PAS** le fichier `.qsl_cache.json`
- Ce fichier évite automatiquement les doublons
