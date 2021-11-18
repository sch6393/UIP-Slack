UIP-Slack
===

### 説明
1. Jobcanから依頼申請を貰うとSlackにメッセージを受信
2. SlackのメッセージからJobcan依頼の内容を読み込む
3. その内容を編集し、Google Calendarに登録
>上記の内容をサイクルする。

<br>

### Slack設定
1. https://app.slack.com/apps-manage/
1. カスタムインテグレーション
1. Appディレクトリを検索で「Incoming Webhook」を検索
1. Slackに追加
1. チャンネルを選択
1. Webhook URL取得
1. チャンネルIDはチャンネル詳細で取得

<br>

### Jobcan設定
1. Jobcan　→　通知設定　→　チャットツール連携
1. 設定値を入力
    ```
    Slack通知設定 ：「通知設定する」をチャック
    Webhook URL   ：Slackで取得したWebhook URL
    メンション設定：Slackで取得したチャンネルID
    ```
1. 「Slackテスト通知」ボタンをクリックして受信確認

<br>

### 問題点
1. いつかはSlack Appに変更しなければならない
1. このProcessを実行する専用PCが要求される
