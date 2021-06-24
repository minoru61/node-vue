# node-vue is to study vue.js
# コンテナ作成例
docker run -it -d --name node-vue -p 8080:8080 -v /Users/minoru/Programs/node-vue:/app node:14-buster

# VSCodeにRemote Containerのプラグインをインストール
Extensionの検索画面で「Remote」とタイプをしてRemote-Containersを探してインストールする

# .devcontainerフォルダとdevcontainer.jsonを作成する
左下のアイコンから、Add Development Container configuration Fileを選択してNode.jsのテンプレートをさがして選択をする。.devlcontainerフォルダに.devcontainer.jsonが作成される

docker-compose.yml
Dockerfile

も同時に作成されるが、コンテナを自分で作った場合は使わないのでとりあえず無視

# .devcontainer.jsonのコンテナ内のワークディレクトリを変更する
コンテナを作成した時に-v オプションでコンテナ内のワーキングディレクトリを設定している。上の例だと/appとなる
"workspaceFolder": "/app"
と設定をする

# コンテナにアタッチする
ContainerのメニューからAttach to Running Containerを選択する

# vueの開発をする
npm install -g @vue/cli
vue create <プロジェクト名>
$ cd my-poject
$ npm run serve
