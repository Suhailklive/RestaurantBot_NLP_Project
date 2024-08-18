Directory structure
===================
backend/: Contains Python FastAPI backend code
db/: contains the dump of the database. you need to import this into your MySQL db by using MySQL workbench tool
dialogflow_assets: Contains Dialogflow assets, such as training phrases and intent configurations.
frontend: Contains the website code, including HTML, and CSS.

Install these modules
======================

pip install mysql-connector
pip install "fastapi[all]"

OR just run pip install -r backend/requirements.txt to install both in one shot

To start fastapi backend server
================================
1. Go to backend directory in your command prompt
2. Run this command: uvicorn main:app --reload

ngrok for https tunneling
================================
1. To install ngrok, go to https://ngrok.com/download and install ngrok version that is suitable for your OS
2. Extract the zip file and place ngrok.exe in a folder.
3. Open windows command prompt, go to that folder and run this command: ngrok http 8000

NOTE: 
- If encountered with a browser warning, install the Google extension 'ModHeader' and set the 'ngrok-skip-browser-warning : true'
- ngrok can timeout. you need to restart the session if you see session expired message.
