# 🤖 Chatbot Reddit sur l'IA et la Data Science

Ce projet a pour objectif de construire un **chatbot intelligent** à partir de conversations Reddit issues de subreddits spécialisés en **Intelligence Artificielle** et **Data Science**. Le modèle est fine-tuné sur **GPT-2 Medium** à partir de dialogues réels pour offrir des réponses cohérentes et naturelles.

---

## 📁 Structure du projet

```
├── extraction_des_donnees.ipynb
├── analyse.ipynb
├── preprocessing.ipynb
├── chatbot.ipynb
├── README.md
├── data/  → données Reddit (disponibles via lien externe)
└── modele/ → modèle fine-tuné (disponible via Drive)
```

---

## 📌 Description des notebooks

### 🔸 `extraction_des_donnees.ipynb`
- Extraction automatique des posts et commentaires à l'aide de **PRAW** (Python Reddit API Wrapper).
- Ciblage de **5 subreddits** centrés sur l'IA et la Data Science : `r/MachineLearning`, `r/datascience`, `r/deeplearning`, `r/artificial`, `r/ArtificialInteligence`.
- Sauvegarde des données sous format brut .

---

### 📊 `analyse.ipynb`
- Analyse exploratoire des posts et commentaires extraits.
- Visualisation des **nuages de mots** sur les thématiques récurrentes.
- **Analyse de sentiment** des messages pour mieux comprendre les tonalités.
- Statistiques descriptives sur la longueur, la fréquence des mots, la distribution des commentaires, etc.

---

### 🧹 `preprocessing.ipynb`
- Nettoyage des textes : suppression des caractères spéciaux, normalisation, etc.
- Filtrage des messages trop courts ou non informatifs.
- Mise au format `.txt` pour l'entraînement GPT-2.

---

### 🧠 `chatbot.ipynb`
- **Tokenisation et vectorisation** des données textuelles.
- Téléchargement du modèle **GPT-2 Medium** via Hugging Face.
- Fine-tuning sur les dialogues Reddit.
- Construction d'une **interface conversationnelle avec Gradio** pour interagir avec le chatbot.

---

## 🗃 Dossiers lourds (données & modèle)

### 📦 Données Reddit
Le dossier `data/` contient l'ensemble des messages extraits (~230 Mo).  
📅 Accès direct : [Lien Drive vers les données](https://drive.google.com/drive/folders/1GED4nMp0PecYyOnp9UcnlPWvsBt25Lwb?usp=sharing)

### 🧠 Modèle Fine-tuné
Le dossier `modele/` contient le modèle GPT-2 fine-tuné (~1.3 Go).  
📅 Accès direct : [Lien Drive vers le modèle](https://drive.google.com/drive/folders/1GED4nMp0PecYyOnp9UcnlPWvsBt25Lwb?usp=sharing)

---

## 🧪 Exécution (sur kaggle conseillé car disponibilité de gpu gratuit pour 30H par semaine)

Pour exécuter le projet (en local) :

1. Cloner ce dépôt :
```bash
git clone https://github.com/Hmd-02/chatbot_RAG_with_Reddit.git
cd chatbot_RAG_with_Reddit
```

2. Télécharger les fichiers `data/` et `modele/` et les placer dans le même repertoire que le script `chatbot` et s'assurer de modifier les chemin d'accès avant d'exécuter


3. Installer les dépendances :
```bash
pip install -r requirements.txt
```

4. Lancer l'interface Gradio :
```bash
python chatbot.ipynb  # ou via Jupyter
```

---

## 💡 Objectifs

Ce projet s’inscrit dans une logique d’apprentissage (projet du cours de NLP) autour de :
- L’**extraction de données web (API Reddit)**.
- Le **prétraitement NLP** avancé.
- Le fine-tuning d’un modèle **transformer préentraîné (GPT-2)**.
- L’analyse de **données conversationnelles** réelles.
- La mise en place d’une interface interactive de **chatbot**.

---

## 📚 Technologies utilisées

- Python, Jupyter Notebooks
- PRAW, pandas, matplotlib, seaborn
- NLTK, transformers (HuggingFace), Gradio
- Google Drive pour la gestion des fichiers lourds

---

## 📢 Contact

Pour toute question, suggestion ou contribution :  
**Auteur :** [Faïçal OUEDRAOGO - Fatimata TALL - Ange DASSI / Hmd-02]  
📧 Email : aide.app.ofch@gmail.com

