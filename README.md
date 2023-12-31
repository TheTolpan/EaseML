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