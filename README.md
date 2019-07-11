#  専門用語

|用語|Bitbucket Pipelines|GitLab CI/CD|CircleCI|
|:-|:-|:-|:-|
|メイン処理|`pipelines:`|`stages:`|`workflows:`|
|最小単位|step|job|job|
|並列処理|`parallel:`を使う|`stage:`に同じ名前をつける|`requires:`で同じjobを処理待ちする|
|ブランチ・プルリクの指定|`pipelines:`に書く|`job:`に`only:`で指定|`only:`にbranch名を指定、設定から`pull request`でのrunを有効にする|
|job,step間でディレクトリを共有する方法|`step:` -> `artifacts:`|`cache:` -> `paths:`|`persist_to_workspace:` -> `paths:`|
|前回のテスト結果からディレクトリをキャッシュする|`step:` -> `caches:`|`artifacts:` -> `paths:`|`save_cache`,`restore_cache:`|
