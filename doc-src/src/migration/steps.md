# 移行ステップ

現行のSlackからZulipへ移行するステップとして以下のようなものを予定しています。

（重要度A〜C案件については、近日中にGitHub Issueかなにかに登録します）

1. [**DONE**] **Zulipにストリームを新設する**
   - `tech talks`
   - `mokumoku`
   - `local communities`
   - `wg/zulip migration`
1. [TODO] **Zulip → Slack連携を設定する**
   - Zulipの主要ストリームに新しいトピックが立ったらSlackへ通知
1. [**DONE**] **`feed`ストリームを追加し、RSSフィードを登録する**（Slackと二重に持つ）
1. [TODO] **ここで、重要度A案件が解決するまで待つ？**
   - 常連メンバーがある程度揃うなら A案件の解決を待たなくてもいいかも
1. [TODO] **一部のSlackチャネルをZulipストリームへ移行する**（試験運用開始）
   - `announce`（新規トピックが立ったらSlackの`announce`へ通知）
   - `beginners`（新規トピックが立ったらSlackの`beginners`へ通知）
   - `questions`（新規トピックが立ったらSlackの`code`へ通知）
1. [TODO] **Slack側の`feed`を停止する**
1. [TODO] **半年ほど経ってから本運用の見極め**
   - よい感触を得られたら本運用とし、Slackの残りのチャネルも移行する
   - その頃までにはモバイルアプリが成熟するなどC案件まで片付いていてほしい


## アクションアイテム

移行に必要なアクションアイテムは現在のところ以下の通りです。（カッコ内は担当者）
このドキュメントではアクションアイテムを更新しづらいので、近日中にGitHub Issueかなにかに登録します。

- (tatsuya6502) Zulip → Slack連携の方法を調査する
- (TBD) 必要ならZulip → Slack連携のしくみを開発する
- (TBD) Zulip → Slack連携を設定する
- (tatsuya6502) [**DONE**] RSSフィード登録の方法を調査する
- (tatsuya6502) [**DONE**] `feed`チャネルにRSSフィードを登録する
