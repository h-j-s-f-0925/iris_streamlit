# 環境構築
- 現在のPythonのパス
    - C:\Anaconda\python.exe
    - C:\Python310\python.exe
    - C:\Users\seiji\AppData\Local\Microsoft\WindowsApps\python.exe

- Dockerを使用してAnacondaでPython環境を管理してみたいとおもった。

- 一旦Anacondaで環境構築することにした

- Anaconda
    - conda env list
    - conda create --name env1 python=3.8
    - activate kikagaku
    - conda install 

- conda install -c conda-forge streamlitが終わらないのはなぜ？
    - conda clean --all して、全部消えた
    - conda clean --allしたらconda installできなくなった
    - conda install conda
    - conda update conda
    - conda install -c conda-forge streamlit
    - streamlit --version

- VSCode で拡張機能のインストール
- 仮想環境をアクティブにするには？
- Ctrl + P でコマンドパレットを開き、Pythonインタープリンターを選択

# Git管理
## GitHub に SSH キーを登録
- ※GitBashで実施

- Step1 : 既に SSH キーを所持していないか確認する
    - ls ~/.ssh
- Step2 : 新たに SSH キーを追加する
    - ssh-keygen -t ed25519 -C "your_email@example.com"
- 実行すると３つのメッセージが出力されます。それぞれ SSH キーの保存場所やパスフレーズの指定についての項目ですが、未記入のまま Enter を押してください。
    - ls ~/.ssh
- Step3 : SSH キーを GitHub に登録する
    - clip < ~/.ssh/id_ed25519.pub
- コピーができたら、GitHub を開きログインし、[右上のプロフィール画像] > [Settings / 設定] > [アクセス] > [SSH キーと GPG キー] の順にクリックし、設定画面を開きます。次に [New SSH key] または [Add SSH key] を選択します。

## Streamlit sharing への登録

## リモートリポジトリの作成
GitHubのダッシュボード上で、New を押し、リモートリポジトリを GitHub 上に作成します。
- リポジトリが作成できたら、表示されている SSH 接続 の URL を使用するので、ここでコピー

## ローカルリポジトリとリモートリポジトリの連携
- git init
- git remote add origin （GitHub上でコピーしたURL
- requirements.txtの追加

## GitHubへのプッシュ
- git add .
- git commit -m "1st commmit"
- git push origin main
