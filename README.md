# PDSProject
## Githubでのプロジェクトの管理とローカルでの作業
1. Githubをインストール
2. プロジェクトをダウンロード & 作業するためのフォルダを作成
3. 右クリック → Git Bash Hereを起動し以下のコマンドを実行
```
git config --global user.name "任意の名前"
git config --global user.email "任意のアドレス"
```
4. Githubのリポジトリを開き、Code → HTTPSタブからURLをコピー
5. 3に引き続き以下のコマンドを実行
```
git clone 4でコピーしたリポジトリのURL(Insert+Shiftでペースト)
```
6. 複製したプロジェクトを編集する時はVSCodeで開いて作業する
7. VScodeのソース管理からコミット
8. 以下のコマンドを実行してリポジトリに作業内容を反映
```
git push
```


