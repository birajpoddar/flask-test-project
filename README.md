# Flask Test Project

## Steps to initialize a Python Flask Project

1. Create a python virtual env

```
python3 -m venv <env_name>
```

2. Activate the virtual env

```
. <env_name>\bin\activate
```

3. Upgrade installed pip

```
pip intall --upgrade pip
```

4. Install Flask

```
pip install flask
```

4. Create a **app.py** for application

```
touch app.py
```

5. Add the following lines for a simple app in **app.py**

```
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return "Hello World"

if __name__ == '__main__':
    app.run()
```

6. Run the application

```
python app.py
```

7. Check the deployed app on http://127.0.0.1:5000
8. Stop the deployed app by clicking `Ctrl+C` on console
9. Create a dependency list

```
pip freeze > requirements.txt
```

10. Init a GIT repo

```
git init
```

11. Create a .gitignore file

```
touch .gitignore
```

12. Add virtual env and os related file to GIT ignore so that they are not pushed to remote host

```
## Virtual Env dir
env

## Mac OS file
.DS_Store
```
