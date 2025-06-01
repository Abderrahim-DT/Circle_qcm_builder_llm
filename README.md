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
