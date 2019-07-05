#  専門用語

|用語|Bitbucket Pipelines|GitLab CI/CD|
|:-|:-|:-|
|メイン処理|`pipelines:`|`stages:`|
|最小単位|step|job|
|並列処理|`parallel:`を使う|`stage:`に同じ名前をつける|
|ブランチ・プルリクの指定|`pipelines:`に書く|`job:`に`only:`で指定|
|1回のテストでファイルを共有する方法|`step:` -> `artifacts:`|`cache:` -> `paths:`|
|前回のテストのキャッシュを引き継ぐ|`step:` -> `caches:`|なし|
|||||