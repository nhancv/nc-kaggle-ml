# kaggle-anomous


### Kaggle: https://www.kaggle.com
### Anomous team: https://medium.com/anomous

#### Download & Install app
https://nteract.io/desktop

#### Install kernal
https://nteract.io/kernels
```
# In .bash_profile
export PYTHON3_ROOT="$PROGRAM_FILES/python/py3_0"
alias python3.setup="python3 -m venv $PYTHON3_ROOT && python3.activate"
alias python3.destroy="rm -rf $PYTHON3_ROOT"
alias python3.activate="source $PYTHON3_ROOT/bin/activate"


# In terminal

## You need setup new env first time
python3.setup

*Note*: new env will be activated after setup automatically

## If the env already setup, you can just active it before working
python3.activate

## Install kernel
(py3_0) ~|⇒ python -m pip install ipykernel
## Install kernel with specific name of env
(py3_0) ~|⇒ python -m ipykernel install --user --name "py3_0" --display-name "Python (3_0)"

## You should deactivate env after working
(py3_0) ~|⇒ deactivate


## View kernel list
(py3_0) ~|⇒ jupyter kernelspec list

## To uninstall kernel
(py3_0) ~|⇒ jupyter kernelspec uninstall <alias>
```

#### Install python libs
```
(py3_0) ~|⇒ pip3 install numpy scipy matplotlib pandas statsmodels scikit-learn IPython seaborn nltk plotly cufflinks lightgbm yellowbrick
```

Install LightGBM on mac

```
#https://github.com/Microsoft/LightGBM/blob/master/docs/Installation-Guide.rst

brew install cmake
brew install libomp
git clone --recursive https://github.com/Microsoft/LightGBM ; cd LightGBM
mkdir build ; cd build
cmake ..
make -j4

cd ../../
rm -rf LightGBM
```

#### Install kaggle
Install cli: https://github.com/Kaggle/kaggle-api
```
pip install kaggle --upgrade

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

