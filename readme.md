
# Guide pour lancer l'application

## Étape 1 : Télécharger le code
1. Téléchargez le code source et placez-le dans un répertoire local de votre choix.
2. Assurez-vous de noter l'emplacement exact du dossier téléchargé.

## Étape 2 : Créer un environnement virtuel
1. Ouvrez un terminal et naviguez dans le dossier où le code a été téléchargé :
   ```bash
   cd path/to/Deployement
   ```
2. Créez un environnement virtuel avec Python 3.12.2 :
   ```bash
   python -m venv .venv
   ```
3. Activez l'environnement virtuel :
   - Sur Windows :
     ```bash
     .venv\Scriptsctivate
     ```
   - Sur macOS/Linux :
     ```bash
     source .venv/bin/activate
     ```

## Étape 3 : Installer les dépendances
Installez les dépendances nécessaires en utilisant le fichier `requirements.txt` :
```bash
pip install -r requirements.txt
```

## Étape 4 : Configurer le fichier `.env`
1. Ouvrez le fichier `.env` situé dans le dossier du projet.
2. Vérifiez et modifiez les chemins pour qu'ils correspondent au dossier où vous avez placé le projet. Voici un exemple de configuration :
   ```env
   # Fichier de configuration, là où seront stockés les devices
   CONF_FILE_PATH=C:\path\to\Deployement\devicesConfiguration\devicesConf.json
   
   # Dossier où seront stockées les données des devices
   DATA_FILE_PATH=C:\path\to\Deployement\devicesJsonData

   # Fichier de correspondance entre les OID et les noms des devices
   CORRESPONDANCE_FILE_PATH=C:\path\to\Deployement\snmp_correspondances.json
   ```

## Étape 5 : Lancer l'application
1. Assurez-vous que l'environnement virtuel est activé.
2. Exécutez le script principal :
   ```bash
   python main2.py
   ```
3. Suivez les instructions affichées dans le terminal pour utiliser l'application.
