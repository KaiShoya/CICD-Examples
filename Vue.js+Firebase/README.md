# 前提条件
masterへのpush、全てのpull requestでCI/CDを動かします。  
下記のプロジェクトで動作を確認済みです。

```bash
$ vue init webpack ci-sample
$ cd ci-sample
$ firebase init
❯◉ Hosting: Configure and deploy Firebase Hosting sites

# FIREBASE_PROJECT_ID
# FirebaseのプロジェクトID
# FIREBASE_TOKEN
$ firebase login:ci
```
