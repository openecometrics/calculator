---
title: Ecometric calculator
emoji: 🌳
colorFrom: indigo
colorTo: pink
sdk: gradio
sdk_version: 3.36.1
app_file: app.py
pinned: false
tags: [climatebase, biocredits, biodiversity, ecometrics]
---

# Bioscore calculator app

This is a simple guide to help you set up and run a Gradio app.

## Prerequisites

- Python 3 installed on your system
- venv module for creating a virtual environment (usually comes with Python)

## Installation

Clone the repository to your local machine:
```bash
git clone https://github.com/your-username/gradio-app.git
cd gradio-app
```

Set up the service account credentials:
- Obtain a service account key file (in JSON format) with the necessary permissions to access any external services required by your Gradio app.
- Save the service account key file as `service_account.json` in the project directory.

Create and activate a virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate
```

Install the required Python packages:
```bash
pip3 install -r requirements.txt
```

## Run the App Locally

To start the Gradio app, execute the following command:

```bash
gradio app.py
```

The app will start running, and you should see output similar to the following:

```
Running on http://127.0.0.1:7860
Open your web browser and visit http://127.0.0.1:7860 to access the Gradio app.
```


## Deploy to Huggingface

The app is hosted a Huggingface space, under the `hf` host and `main` branch. 

To push changes from main branch to Huggingfage, run:

```bash
git push hf main
```

You'll see the app's response in `https://huggingface.co/spaces/openbio/calculator`

❗Note: There's no dev nor staging environment, nor CI. Every push will immediately build and go live.


## Customization

Feel free to modify the app.py file to customize the behavior and appearance of your Gradio app. You can add or remove input and output interfaces, change their appearance, or include additional functionality as per your requirements.

## Feedback

If you encounter any issues or have any questions or suggestions, please don't hesitate to open an issue on the GitHub repository. We appreciate your feedback and contributions!

## License

This project is licensed under the MIT License.
