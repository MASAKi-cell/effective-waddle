# Vue.js + Firebaseで作成した動画検索のポートフォリオサイトを作成しました。 #

### このポートフォリオサイトを制作した背景
日々のビジネスマンの情報収集や学習の助けになればと思いこのアプリを作成しました。

・サイトタイトル名：Study-Tube<br>
　URL ：https://english-tube-c340d.web.app/
 <br>
　GitHub：https://github.com/MASAKi-cell/Study-Tube

・テスト用アカウン<br>
　メールアドレス：bje@gmail.com <br>
　パスワード　　：English
<br>　※ユーザー管理はfirebaseのAuthenticationを使用してます。



### 目的
コロナの影響で、リモートワークなど家にいる時間が増えました。家にいる間、様々な情報やスキルを学習する助けになればと思い、動画で学べる学習アプリ「Study-Tube」を作成しました。


### 使用技術
・フロントエンド：Vue.js(VueRouter,Vuex,Vuetify,axios)、HTML、Sass
・バックエンド　：Firebase(Hosting,Authentication)


### 主な機能一覧
・会員登録、ログイン、ログアウト、Googleアカウントのログイン機能
・Youtube Video APIから動画をキーワード検索、一覧表示



### こだわりポイント
・ Vue.js上のデータフローを管理するためVuexを使用
・ シングルページアプリケーションを実現するためのVue Router使用
・ Vue.jsの開発環境を素早く立ち上げることができるVue CLI使用
・ Firebase Authenticationを使用したGoogleアカウント認証機能
・ Firebase Hostingを使用したアプリケーションの公開
・ Youtube APIを実装
・ コードはGitHubで管理
・ ヘッダー部のボタンはハンバーガーメニューを実装しレスポンシブに対応してます。



#### 1. ファーストビュー　
・ 最初にアクセスすると本サイトの説明文が記載された画面が現れます。
・ ヘッダーはvue-routerを使用し、router-linkで選択した画面が現れます。

#### 2.新規会員登録/ログイン機能
・ ヘッダーの右側に会員登録機能、ログイン機能のボタンを配置しました。
・ ログインすると、動画検索や学習記録の欄が表示されます。
・ 新規会員登録にはサーバーとHTTP通信を行うためにaxiosを使用しました。
　 既に新規登録が完了している場合は、ログインボタンを押して登録したメールアドレスとパスワードを入力してログインします。
・ ログインユーザーはfirebaseのAuthenticationを使用してユーザーを管理しています。

#### 3.google アカウントログイン機能
・ googleアカウントでのログイン機能も追加しました。
・ stateでlogin_userを格納し、actionを使用してログイン、ログアウトの状態を管理しています。

#### 4.動画検索
・ Youtube APIから取得した動画を表示させることができます。
・ 検索フォームからキーワードを入力して動画を検索することができます。



### 開発を通じて学んだこと
・firebaseの使い方
　認証、デプロイといったバックエンドの実装がfirebaseを使って出来るようになりました。

・Vuexの使い方
　最初はVuexについて苦手意識がありましたが、実際に使用してみると色々な機能が実装できることが分かりました。

・Vue.jsにおけるSPAの作り方
　SPAの下準備から各ページ作成・Vou-router調整ができるようになりました。



### 今後実装していきたい機能
・ 条件を絞り込んだ検索機能
・ いいね機能
・ お気に入りをストックする機能



### 参考にした教材
公式ドキュメント
・axiosを利用したAPI使用例
・認証付きの簡易チャットを作る！
　⇒ アプリを作成する為に、まずは公式のドキュメントを参考にしました。

Vue.jsにおけるSPAの作り方
・Vue.js】【SPA】の作り方をわかりやすくまとめてみた【初心者向け】
　⇒ SPAについて詳しく記載されたサイトです。

created, mountedのライフサイクルフック
vue.jsのcreatedとmountedの違いを目で見て理解
⇒ vue.jsのcreatedとmountedの違いが判りませんでしたが、このサイトを見て理解が深まりました。

Vue.js参考書籍&動画学習　
・Vue.jsのツボとコツがゼッタイにわかる本
　⇒ Vue.jsの事が丁寧に解説されており、Vue.jsの初心者にとってはちょうど良い内容かと思います。
　
・Udemy 超Vue.js 2 完全パック (Vue Router, Vuex含む>
　⇒ Vue JSの基礎から、仮想DOM、Vue CLIを使った開発方法などVue.jsの全体的な内容を学ぶことができました。



### 反省点
・axiosを利用したHTTPリクエストやサーバーサイドの知識を深めていく必要があると感じました。
・これまで、GitHub DesktopでGitHubにアクセスしてましたが、今回はコマンドプロンプトを使用してコードを管理しました。
　ただやり方がわからず、もっと理解を深めていく必要があると感じました。
・Vuexを使用した状態管理についてもっと学習していきます

