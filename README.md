# Tkinterを使ったサイト監視ツール


### インストール
````console:bash
pip install -r install.txt
````

### 前提環境
````console:bash
python v3.9+
````

## exe化コマンド

### pyinstaller
.specファイルを利用して詳細設定込みでexe化
※別途pyinstallerのインストール、ビルドツールの設定が必要
````console:bash
pyinstaller App.spec
````
### nuitka
pyinstallerのビルドに問題があった場合はこっちで試す
※別途nuitkaのインストールが必要
````console:bash
nuitka --standalone --windows-disable-console --enable-plugin=tk-inter --include-package-data=cssutils --include-package-data=selenium Application.py
````
