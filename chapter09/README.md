## 运行步骤
```
cd ./chapter09
python test_watchlist.py
coverage run --source=app test_watchlist.py
coverage report
coverage html
```
## 说明
运行coverage run --source=app test_watchlist.py命令，可能会提示ModuleNotFoundError: No module named 'app'，那是因为当前目录没有加到PYTHONPATH里面，这时需要在venv\Lib\site-packages目录底下新一个后缀为.pth的文件 ，文件名随便，内容为当前目录。
