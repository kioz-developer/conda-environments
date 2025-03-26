
### basic conda environment for text to speech


#### Create
> conda env create -f tts/environment.yml

#### Activate
> conda activate tts

#### Start Jupyter
> jupyter lab



### basic conda environment to data analysis


#### Create
> conda env create -f data/environment.yml

#### Activate
> conda activate data

#### Start Jupyter
> jupyter lab



### basic environment to use Diffusers

#### Create
> conda env create -f diffusers/environment.yml

#### Activate
> conda activate diffusers

#### Disable telemetry logging (Linux)
> export DISABLE_TELEMETRY=YES
#### Disable telemetry logging (Windows)
> set DISABLE_TELEMETRY=YES


#### Start Jupyter
> jupyter notebook




### basic conda environment for linear algebra


#### Create
> conda env create -f linear_algebra/environment.yml

#### Activate
> conda activate linear_algebra

#### Start Jupyter
> jupyter lab




### basic conda environment for NLP-BERT of Hugging Face Transformers


#### Create
> conda env create -f nlp_bert/environment.yml

#### Activate
> conda activate nlp_bert

#### Start Jupyter
> jupyter lab




### basic conda environment to webscraping


#### Create
> conda env create -f scraping/environment.yml

#### Activate
> conda activate scraping

#### Start Jupyter
> jupyter lab




### basic conda environment to use Flask


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