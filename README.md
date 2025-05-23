# FixYourNetflix-TUFIQoE-2022

Chrome extension and Python/flask REST API for QoE experiment with high [mundel realism](https://dictionary.apa.org/mundane-realism) using Netflix streaming platform. 

Similiar to the [YourNetflixOurLab](https://github.com/navuyi/YourNetflixOurLab-TUFIQoE-2022.git). Includes modifications of Netflix's Cadmium Playercore script:
- changing buffer size
- enabling bitrate menu allowing manipulations of video (and audio) quality.

## Technology stack
Frontend (Chrome extension)
- Webpack
- React
- Typescript


Backend
- Python (Flask)
- Sqlite3

## Installing and Running

### Procedures:

1. Check if your [Node.js](https://nodejs.org/) version is >= **14**.
2. Clone this repository.
3. Go to /extension folder.
4. Run `npm install` to install the dependencies.
5. Run `npm run build`
6. Load your extension on Chrome following:
    1. Access `chrome://extensions/`
    2. Check `Developer mode`
    3. Click on `Load unpacked extension`
    4. Select the `build` folder.
7. Run backend:
    1. cd into `backend` directory
    2. run `python database/init.py` to initialize SQLite3 database
    3. Create virtual environment `python -m venv venv` in main catalog
    4. Activate the python virtual environment by running OS compatible command. On macOS: `source venv/bin/activate`, on Windows: `venv\Scripts\activate.bat`
    6. Install requirements `pip install -r requirements.txt` in backend catalog
    7. On macOS run `source start-mac.sh` || on Windows `.\start-windows.bat`
8. Happy hacking.

# Acknowledgments

The software development leading to this repository has received funding from the Norwegian Financial Mechanism 2014-2021 under project 2019/34/H/ST6/00599.

