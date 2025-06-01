# llm-qcm-project

Générateur de QCM fine-tuné à partir de documents pédagogiques.

## Objectifs
- Extraction automatique de contenu depuis PDF/DOCX
- Annotation de données pour fine-tuning
- Fine-tuning de modèle LLM avec LLaMA-Factory
- Export vers une API pour intégration backend/frontend

## Structure
- `data/` : données brutes, traitées, annotées
- `scripts/` : outils d'extraction, annotation, préparation
- `configs/` : fichiers YAML pour le fine-tuning
- `inference/` : test d'inférence après entraînement


llm-qcm-project/
├── data/
│   ├── raw/                  # Fichiers bruts (PDF, DOCX, etc.)
│   ├── processed/            # Textes extraits
│   └── annotated/            # Fichiers .jsonl annotés à la main
├── scripts/
│   ├── extract_text.py       # Extraction depuis PDF, DOCX
│   ├── annotate.py           # Aide à l'annotation semi-auto
│   ├── prepare_dataset.py    # Formatage final pour le fine-tuning
│   └── validate_dataset.py   # Vérification syntaxique et structurelle
├── configs/
│   └── finetune_config.yaml  # Config YAML pour LLaMA-Factory
├── docker/
│   └── Dockerfile            # pour la portabilite
├── inference/
│   └── api.py                # l'interface pour communicqtion avec back/front end
├── .gitignore
├── Makefile                  # Pour exécuter rapidement les étapes
├── README.md
└── .github/
    └── workflows/
        └── validate_dataset.yml  # GitHub Actions pour valider les .jsonl

