# memo

## Docker

- 全コンテナの停止：`docker stop $(docker ps -q)`
- 全コンテナの削除：`docker rm $(docker ps -q -a)`
- 全イメージの削除：`docker rmi $(docker images -q)`
- Dockerが使っているローカルの容量確認：`docker system df`
- ビルドイメージの削除：`docker builder prune`
    - イメージを削除してもキャッシュが残っているので容量は空かない。キャッシュを削除したいときに使う

## devcontainer

- git push origin mainできなくなったら
    - macのコンソールより`ssh-add $HOME/.ssh/id_rsa`を実行。
        - `id_rsa`の部分はgithubに登録した公開鍵の対である秘密鍵