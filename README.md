# SSH Login Teraterm Macro


## Usage

### Files
#### Macro files
- login.ttl
- commands.ttl

#### Data files
- commandslist.csv
- hostlist.csv
- password.dat

### ログイン
1. `hostlist.csv`に接続情報や接続時投入コマンドファイルパス等を記載する
2. `macro_login.ttl`を実行する
3. ダイアログが表示されるので接続したい機器を選択して接続する
4. 接続後`hostlist.csv`に記載のコマンドファイルを読み込みそのファイルのコマンドが自動で投入される

#### パスワード
初回接続時パスワード入力ダイアログが表示される
パスワードは難読化され`password.dat`に格納され、次回以降はそのファイルを参照してログインする

### コマンド投入
1. `commandslist.csv`にコマンドファイルパスを記載する
2. ログイン中に`macro_commands.ttl`を実行する
3. `commandslist.csv`に記載のコマンドファイルを読み込みそのファイルのコマンドが自動で投入される

## Requirements
- Tera Term 4.78 >=

## References
- [Tera Term Home Page](https://ttssh2.osdn.jp)
- [Tera Termマニュアル](https://ttssh2.osdn.jp/manual/4/ja/)

## License
MIT License Copyright (c) 2022 yuyosy