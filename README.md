# 美女マップ(クライアント)
 バイト先で働く美女からバイトを探すサービス
-----
* index.html
初期画面

* choice1.html, choice2.html, choice3.html
初期設定画面

* map.html
マップ画面

* js
 - profile-set.js
　　初期設定画面で女の子を選択したときに好み情報をPOST

 - mapdisplay.js
　　地図表示処理、情報ウィンドウ配置処理を実装

 - location.js
　　現在地情報を取得

 - init-user.js
　　index.htmlにてスタートボタンプッシュ鵜時に実行
　　ユーザ情報がある場合はマップ画面へ、ない場合は初期設定画面へ遷移

* css
 - for_init.css
初期設定画面のスタイル
 - login_style.css
index.htmlのスタイル
 - map_style.css
map.htmlのスタイル


ーーーーーー
***
---

2013/12/13
・各ファイルにコメントを追加
・web-native.js ⇒ PCからアクセスの場合はテスト用IDを返すなどの対応を追加
・bootstrap.cssを使用するように変更
・『この美女をお気に入りに登録した人は他にこんな美女を登録しています。』表示のためにカルーセルを追加


2013/12/10
・post.js⇒send.jsに名称変更
・data.jsonp⇒内容を修正
・util.js⇒URLから?以降のパラメータを取得する処理
・web-native.js⇒Webとネイティブの連携処理
・favo.js, detail.js⇒最低限jsonpファイルからデータを取得して表示するように修正

2013/12/07
・css/main.css
	共通スタイル + お気に入り画面のスタイル + 概要画面のスタイルを記載
・data.jsonp
	テスト用のデータを記載
・detail.html
	概要画面のhtml
・favo.html
	お気に入り画面のhtml
・img
	girl: テスト用の画像
	b027.jpg: 背景用の画像
	back.png: メニューを閉じるボタン用の画像
	list.png: メニュー表示ボタン用の画像
・js
	blocksit.min.js: ピンタレスト風の表示に使用
	detail.js: 概要画面の作成用
	favo.js: お気に入り画面の作成用
	gistfile1.js: 画像の読み込み後に処理を実行するために使用(ピンタレスト画面用)
	jquer-2.0.2.js: jQueryファイル(最新版)
	main.js: 共通処理を記載
	post.js: サーバ通信用の関数を記載(現在はjsonpファイル読み込み用に特化しています)
