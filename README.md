# kaggle-anomous


### Kaggle: https://www.kaggle.com
### Anomous team: https://medium.com/anomous

#### Download & Install app
https://nteract.io/desktop

#### Install kernal
```
python -m pip install ipykernel virtualenv
python -m ipykernel install

python3 -m pip install ipykernel virtualenv
python3 -m ipykernel install
```

#### View kernel list
```
jupyter kernelspec list
```

#### Install python libs
```
pip3 install numpy scipy matplotlib pandas statsmodels scikit-learn IPython seaborn nltk plotly cufflinks
pip install numpy scipy matplotlib pandas statsmodels scikit-learn IPython seaborn nltk plotly cufflinks
```

#### Install kaggle
Install cli: https://github.com/Kaggle/kaggle-api
```
pip install kaggle —upgrade

# Auth
touch ~/.kaggle/kaggle.json
chmod 600 ~/.kaggle/kaggle.json

# Update kaggle.json file
# Get api token key at https://www.kaggle.com/nhancv/account
export KAGGLE_USERNAME=nhancv
export KAGGLE_KEY=xxxxxxxxxxxxxx
```

#### Submit competition
```
kaggle competitions submit -c titanic -f submission.csv -m "submit solution"
```

#### Execute .ipynb file
```
# Install jupyter, nbconvert
pip install ipython jupyter nbconvert

# Convert to py script
jupyter nbconvert --to script titanic.ipynb

# Run py script
ipython titanic.py

````

