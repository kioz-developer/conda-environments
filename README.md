
### basic jupyter environment to data analysis


#### Create
> conda env create -f data/environment.yml

#### Activate
> conda activate data

#### Start Jupyter
> jupyter notebook


### basic jupyter environment to webscraping


#### Create
> conda env create -f scraping/environment.yml

#### Activate
> conda activate scraping

#### Start Jupyter
> jupyter notebook


### basic environment to use Flask


#### Create
> conda env create -f flask/environment.yml

#### Activate
> conda activate flask

#### Create basic app.py
```
from flask import Flask
from flask import jsonify

app = Flask(__name__)

@app.route('/')
def index():
    return 'Api is running', 200

if __name__ == "__main__":
    app.run(debug=True)
```

#### Start using Flask
> flask run --port=5001