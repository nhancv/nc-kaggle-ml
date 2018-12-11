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
pip3 install numpy scipy matplotlib pandas statsmodels scikit-learn IPython seaborn
pip install numpy scipy matplotlib pandas statsmodels scikit-learn IPython seaborn
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



