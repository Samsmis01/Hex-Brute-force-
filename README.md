
# **Hex-Brute-Force**

**Hex-Brute-Force** est un outil de test de force brute conçu pour démontrer les principes de sécurité en matière de mots de passe. Ce script génère une liste de mots de passe aléatoires et simule une attaque par force brute sur un système fictif. Il est conçu à des fins éducatives et ne doit pas être utilisé à des fins malveillantes.

---

## **Fonctionnalités**

- Génère une liste de mots de passe aléatoires.
- Simule une attaque par force brute sur un système fictif.
- Prend en charge les mots de passe avec des lettres, des chiffres et des caractères spéciaux.
- Enregistre les résultats dans un fichier texte.

---

## **Installation**

### **Prérequis**

- Python 3.x installé sur votre système.
- Les modules suivants doivent être installés :
  - `random`
  - `string`
  - `os`

### **Étapes d'installation**

1. **Cloner le dépôt** :
   Ouvrez un terminal et exécutez la commande suivante pour cloner le dépôt :
   ```bash
   git clone https://github.com/Samsmis01/Hex-Brute-force-.git
   ```

2. **Accéder au dossier du projet** :
   ```bash
   cd Hex-Brute-Force
   ```

3. **Exécuter le script** :
   Exécutez le script Python pour générer la liste de mots de passe :
   ```bash
   python generate_wordlist.py
   ```
   
## **Utilisation du script depuis Termux**

### **Étape 1 : Installer Termux**
Si vous n'avez pas encore Termux, installez-le depuis le **Google Play Store** ou **F-Droid**.

---

### **Étape 2 : Mettre à jour et installer les dépendances**
1. Ouvrez Termux.
2. Mettez à jour les paquets existants :
   ```bash
   pkg update && pkg upgrade
   ```
3. Installez Python et Git :
   ```bash
   pkg install python git
   ```

---

### **Étape 3 : Cloner le dépôt Hex-Brute-Force**
1. Clonez le dépôt GitHub dans Termux :
   ```bash
   git clone https://github.com/Samsmis01/Hex-Brute-force-.git
   ```
2. Accédez au dossier du projet :
   ```bash
   cd Hex-Brute-Force
   ```

---

### **Étape 4 : Exécuter le script**
1. Exécutez le script pour générer la liste de mots de passe :
   ```bash
   python generate_wordlist.py
   ```
2. Le fichier `Worldlist.txt` sera créé dans le dossier **Téléchargements** de votre appareil Android.

---

### **Étape 5 : Localiser le fichier généré**
1. Ouvrez l'application **Fichiers** ou **Gestionnaire de fichiers** sur Android.
2. Accédez au dossier **Téléchargements**.
3. Recherchez le fichier `Worldlist.txt`.

---

### **Étape 6 : Personnaliser le script (optionnel)**
Si vous souhaitez modifier le script (par exemple, changer le nombre de mots de passe ou le dossier de sortie), suivez ces étapes :

1. Ouvrez le script dans Termux avec un éditeur de texte comme `nano` :
   ```bash
   nano generate_wordlist.py
   ```
2. Modifiez les variables suivantes :
   - Pour changer le nombre de mots de passe :
     ```python
     generate_wordlist(filename, num_passwords=200)  # Génère 200 mots de passe
     ```
   - Pour changer le dossier de sortie :
     ```python
     downloads_path = "/storage/emulated/0/Documents/"  # Change le dossier de sortie
     ```
3. Enregistrez et quittez (`Ctrl + O` pour enregistrer, `Ctrl + X` pour quitter).

---

### **Étape 7 : Réexécuter le script**
Après avoir personnalisé le script, réexécutez-le :
```bash
python generate_wordlist.py
```

---

## **Exemple de sortie dans Termux**

Lorsque vous exécutez le script, vous verrez une sortie similaire à ceci :
```
La liste de 170 mots de passe a été générée et enregistrée dans '/storage/emulated/0/Download/Worldlist.txt'.
```

---

## **Résolution des problèmes**

### **1. Permission refusée**
Si Termux n'a pas accès au stockage externe, accordez-lui les permissions nécessaires :
1. Ouvrez les **Paramètres** de votre appareil Android.
2. Allez dans **Applications** > **Termux** > **Permissions**.
3. Activez l'accès au **Stockage**.

### **2. Module manquant**
Si un module Python est manquant, installez-le avec `pip` :
```bash
pip install nom_du_module
```

---

