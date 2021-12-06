Demo: Web Chat with Firestore
=============================

A simple web application of real time chatting with Cloud Firestore.

## Getting started

English:

1. Create Firebase project and configure.
  * Open [Firebase Console](https://console.firebase.google.com) and create your new project.
  * Click the icon like **</>** on the top area.
    Or click a gear icon on the left top and go to **Project settings**, then click the icon like `</>` on the **General** tab.
  * Register app and then copy your `const firebaseConfig = { ... }` with your configuration.
  * Paste copied configuration under the `TODO` comment in `templates/index.html`.
2. Enable Firestore.
  * On Firebase console, click **Firestore Database** on the left menu.
  * Click the **Create database** button.
  * Choose **Start in test mode** and click **Next** button.
  * Choose a location where you like to deploy your app to, and click **Enable** button.
3. Deploy the app to App Engine.
  * Configure gcloud with your project ID. Run `gcloud config set project YOUR-PROJECT-ID`.
  * Run `gcloud app deploy`.
  * When an error could occur, it should be like the following.
    * ERROR: (gcloud.app.deploy) Error Response: [7] Access Not Configured. Cloud Build has not been used in project YOUR-PROJECT-ID before or it is disabled. Enable it by visiting https://console.developers.google.com/apis/api/cloudbuild.googleapis.com/overview?project=YOUR-PROJECT-ID then retry. If you enabled this API recently, wait a few minutes for the action to propagate to our systems and retry.
  * Open this URL.
  * Enable billing to the project and enable the Cloud Build API (`cloudbuild.googleapis.com`).
  * Run `gcloud app deploy` again.
4. Enjoy your chat app with the issued URL!

Japanese:

1. Firebase プロジェクトの作成と設定
  * [Firebase コンソール](https://console.firebase.google.com)を開いて、新しいプロジェクトを作成してください。
  * 上部に表示されている **</>** アイコンをクリックしてください。
    もしくは、左メニュー上部の歯車アイコンをクリックして **プロジェクトの設定** から、**全般** タブの **</>** アイコンをクリックしてください。
  * アプリを登録して、あなたの設定を含む `const firebaseConfig = { ... }` をコピーしてください。
  * コピーした設定を `templates/index.html` の `TODO` コメントの下にペーストしてください。
2. Firestore の有効化
  * Firebase コンソールで、左メニューの **Firestore Database** をクリックしてください。
  * **データベースの作成** ボタンをクリックしてください。
  * **テストモードで開始する** を選択して **次へ** ボタンをクリックしてください。
  * アプリケーションをデプロイしたいロケーションを選択して、**有効にする** ボタンをクリックしてください。
3. App Engine へのデプロイ
  * 次のコマンドで gcloud コマンドにプロジェクトを設定してください。 `gcloud config set project YOUR-PROJECT-ID`
  * `gcloud app deploy` コマンドを実行してください。
  * 次のようなエラーが表示される場合があります。
    * ERROR: (gcloud.app.deploy) Error Response: [7] Access Not Configured. Cloud Build has not been used in project YOUR-PROJECT-ID before or it is disabled. Enable it by visiting https://console.developers.google.com/apis/api/cloudbuild.googleapis.com/overview?project=YOUR-PROJECT-ID then retry. If you enabled this API recently, wait a few minutes for the action to propagate to our systems and retry.
  * この URL をブラウザで開いてください。
  * プロジェクトに対して課金を有効化して、Cloud Build API (`cloudbuild.googleapis.com`) を有効化してください。
  * もう一度 `gcloud app deploy` を実行してください。
4. 発行されたURLにアクセスしてください。
