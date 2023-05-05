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

