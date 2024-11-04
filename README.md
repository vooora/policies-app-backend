# Our App
See the demo video for our application here
[https://drive.google.com/drive/folders/1sX0ja2krj693XlLQvvaxrN1CXvJG13rj](https://drive.google.com/drive/folders/1sX0ja2krj693XlLQvvaxrN1CXvJG13rj)
or download from here:
[https://github.com/vooora/policies-app-backend/releases/tag/v1](https://github.com/vooora/policies-app-backend/releases/tag/v1)

# Our tests and results
See the testing_and_results directory to see our test queries and their corresponding answers upon running the backend. The time taken per query are also listed in the time_taken_per_query.pdf file.

# Policies Sparkle Project Full Application
First clone the repository and navigate into your directory.
```
git clone https://github.com/vooora/policies-app-backend.git
cd policies-app-backend
cd client
```
Install dependencies.
```
flutter pub get
```
Ensure you have a device connected, then run the application.
```
flutter run
```


# Policies Sparkle Project Backend

This Backend has been written in Flask and has been Deployed on [[Render](https://policies-app-backend.onrender.com/)](https://policies-app-backend-nlvo.onrender.com). The dataset is the sparkle_schemes directory. 

To run the only backend locally:

First install the `virtualenv` library from PyPI:
```
pip install virtualenv
```
Next, create a virtual environment on python using:

```
python -m venv env
```
or as below, depending on the operating system of the user
```
python3 -m venv env
```

After creating the virtual environment, run the following to activate the virtual environment:

```
source env/bin/activate
```

Upon activating the virtual environment, the user can run the following commands to get the application up and running:

```
pip install -r requirements.txt
python3 app.py #or python app.py 
```

The application should now be running on the localhost with the default port number of 5000.

The deployment version of the application is a WGSI server which uses the `gunicorn` library and it can be run using the command:
```
gunicorn app:app
```
Note that the above command will not work on native windows and requires Windows Subsystem For Linux(WSL) in order to work properly
