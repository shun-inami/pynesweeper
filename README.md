# pynesweeper
Pythonでマインスイーパーを作って遊ぶだけです

## 開発環境について
基本的にDocker上にPython環境を用意して作業します。

### Dockerコマンド
```Shell
docker run -d -it -v "$(pwd):/app" --name pynesweeper python:3.9
docker exec -it pynesweeper /bin/bash
docker stop pynesweeper
docker start pynesweeper
```
※ カレントディレクトリは、このリポジトリをクローンしたルートディレクトリでどうぞ<br>
`$(pwd)`にしているので、変なディレクトリで動かそうとするとソースが入りません。

### Tips
- リポジトリのルーテディレクトリで`code .`とコマンド実行すると、いい感じにVScodeが立ち上がってくれるので便利です。
