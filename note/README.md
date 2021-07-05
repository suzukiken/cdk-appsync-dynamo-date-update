+++
title = "AppSync ResolverでDynamo DBの更新日時をアップデートする"
date = "2021-04-27"
tags = ["AppSync"]
+++

AppSyncのDynamo DBをデータソースにしたresolverで、よくRDBMSでやるような、

* created_datetime: アイテム作成時の日時を保持
* updated_datetime: アイテム更新時の日時を保持

というフィールドを持たせて、日時は自動で初期値が設定され、更新がされるという仕組みを作ってみた。

[Githubのリポジトリ](https://github.com/suzukiken/cdkappsync-dynamo-date-update)


