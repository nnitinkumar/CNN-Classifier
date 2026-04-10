# CNN Classifier

An end-to-end image classification pipeline built with a modular, production-ready architecture. The project follows software engineering best practices with configurable components, DVC for pipeline management, and CI/CD via GitHub Actions.

## Project Structure

```
CNN-Classifier/
├── src/cnnClassifier/
│   ├── components/       # Data ingestion, model training, evaluation
│   ├── config/           # Configuration management
│   ├── constants/        # Project constants
│   ├── entity/           # Data classes and config entities
│   ├── pipeline/         # Training and prediction pipelines
│   └── utils/            # Utility functions
├── config/               # YAML configuration files
├── research/             # Jupyter notebooks for experimentation
├── templates/            # HTML templates (for Flask app)
├── .github/workflows/    # CI/CD pipeline
├── dvc.yaml              # DVC pipeline definition
├── params.yaml           # Hyperparameters
├── main.py               # Entry point
├── setup.py              # Package setup
└── requirements.txt      # Dependencies
```

## Key Design Decisions

- **Modular architecture** — each stage (data ingestion, model training, evaluation) is an independent component
- **Configuration-driven** — all hyperparameters and paths are managed through YAML configs, not hardcoded
- **DVC pipeline** — reproducible ML pipeline with data version control
- **Package structure** — installable as a Python package via `setup.py`

## Tech Stack

`Python` `TensorFlow/Keras` `DVC` `Flask` `GitHub Actions`

## Setup

```bash
git clone https://github.com/nnitinkumar/CNN-Classifier.git
cd CNN-Classifier
pip install -r requirements.txt
python main.py
```

## License

MIT
