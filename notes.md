1. Install modules 

```shell 
pip3 install flask flask-sqlalchemy
```

2. Basic Flask Server 

app.py

```python 
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return "Hello, world!"  

if __name__ == "__main__":
    app.run(debug=True)
```

run `python app.py`

3. Static Templates 

- Create `templates` folder and create index.html file inside it and put some code there.  

code 

```python 
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def index():
    return render_template('index.html') 

if __name__ == "__main__":
    app.run(debug=True)
```   

https://youtu.be/Z1RJmh_OqeA?t=909
