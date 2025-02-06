# AI-QA-System

##  Description
Système de questions/réponses alimenté par l'IA qui permet l'ingestion de fichiers PDF, la création d'embeddings à l'aide de modèles de transformation de texte, et la génération de réponses pertinentes en fonction des informations contenues dans les documents. Ce projet utilise les technologies suivantes :

- **LangChain** : pour la gestion des documents et des vecteurs.
- **Sentence-Transformers** : pour l'encodage de texte en vecteurs.
- **ChromaDB** : pour le stockage des embeddings dans une base de données vectorielle.
- **DeepSeek API** : pour la génération des réponses par IA en fonction du contexte extrait des documents.


## Fonctionnalités

1. **Chargement de documents PDF** : Permet d'extraire le contenu d'un fichier PDF pour traitement ultérieur.
2. **Découpage du texte en morceaux** : Divise le texte extrait en morceaux afin de faciliter la gestion des embeddings.
3. **Embeddings de documents** : Utilise le modèle `all-MiniLM-L6-v2` pour créer des embeddings des documents.
4. **Stockage des embeddings dans ChromaDB** : Les embeddings sont stockés dans une base de données vectorielle pour des recherches rapides.
5. **Recherche de documents pertinents** : Recherche les documents les plus pertinents en fonction de la requête de l'utilisateur.
6. **Génération de réponses IA** : Utilise l'API DeepSeek pour générer une réponse pertinente en utilisant le contexte des documents récupérés


##  Installation

1. **Cloner le dépôt Git**
   ```bash
   git clone https://github.com/El-Aoud-Sabah/AI-QA-System
   cd AI-QA-System
   ```
2. **Créer un environnement virtuel (optionnel mais recommandé)**
   ```bash
   python -m venv myenv
   myenv\Scripts\activate  # Pour Windows
   ```
3. **Installer les dépendances**
   ```bash
   pip install -r requirements.txt
   ```
4. **Créer un fichier `.env` pour stocker la clé API**
   - Crée un fichier `.env.txt` dans le répertoire principal et ajoute :
     ```
     API_KEY='VOTRE_CLE_API'
     ```

##  Utilisation
1. **Exécuter le script**
   jupyter notebook Q&Asystem.ipynb
   
2. **Suivre les instructions**
   - Entrer le chemin du fichier PDF
   - Poser une question en lien avec le document
   - Taper `changer` pour analyser un autre fichier

## Structure du projet

📁 project_root/

│-- Q&Asystem.ipynb  # Code principal

│-- requirements.txt  # Dépendances

│-- .env  # Clé API (non inclus dans Git)

│-- README.md  # Documentation



