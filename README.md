# reference
- [Python3からC++の関数を呼び出す](https://qiita.com/taroc/items/fc854340a5e498ceb07d)

# setup
```
sudo apt-get -y install python3-venv python3-dev
python3 -m venv venv/
source venv/bin/activate
pip install cython
python setup.py build_ext
```

# usage
- symlink to current directory
```
ln -s build/lib.linux-x86_64-3.6/calc.cpython-36m-x86_64-linux-gnu.so .
```
- write main.py
```
import calc
print(calc.add(1, 1))
```
- run
```
$ python main.py
2
```
