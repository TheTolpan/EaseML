# EaseML

SWP: Usable Machine Learning

This is our current project structure:

├── src                         # All source code for the application \
│   ├── app                     # Flask web application \
│   │   ├── __init__.py         # Initializes the Flask app \
│   │   ├── templates           # HTML templates for the web pages \
│   │   ├── static              # Static files (CSS, JS, images) \
│   │   ├── routes              # Flask routes (views) \
│   │   └── utils               # Utility functions, helpers \
│   │ \
│   ├── ml                      # Machine learning related code \
│   │   ├── models              # ML model definitions (using PyTorch) \
│   │   ├── trainers            # Training routines and logic \
│   │   ├── monitors            # Code to monitor training (accuracy, loss, etc.) \
│   │   └── exporters           # Functionality for exporting trained models \
│   │ \
│   └── common                  # Common utilities and shared code \
│
├── config                      # Configuration files for the application \
├── resources                   # Resources for the application \
│   └── data                    # Data directory (can be .gitignored if large) \
├── tests                       # Tests for both app and ML code \
├── docs                        # Documentation for the project \
├── scripts                     # Scripts for setup, deployment, etc. \
│ \
├── .gitignore                  # Files and folders to be ignored by Git \
├── README.md                   # Project overview and setup instructions \
├── LICENSE                     # License information \
├── requirements.txt            # Python dependencies \
└── run.py                      # Script to run the Flask app \


1. Install the requirements into a conda environment
```
conda create --name EaseML --file requirements.txt
```

2. Activate Conda environment

```
conda activate EaseML
```

3. Run the app

```
python run.py
```


The training_config.json in /config needs to have this format:

```
{
    "optimizer_params": {
        "type": "SGD",
        "args": {
            "lr": 0.3,
            "momentum": 0.5
        }
    },
    "batch_size": 256,
    "model_training": 1
}
```