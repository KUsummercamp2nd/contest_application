### 2019年度のストップウォッチプログラム

HTMLもJavaScriptも一切知らない不肖TamagoTorisugiが3日で書いたもので，読みにくい・分かりにくい箇所が多々あると思いますがご了承ください．

####動作環境
VSCodeとGoogle Chromeで動作確認しています．
VSCodeでhtmlを見る手順は https://qiita.com/84zume/items/476a29264fdc98d98201 を参考にしてください，



####準備

dataフォルダ下に，name_register.csvを置く．
name_register.csvは，各チームの名前と各レーサーの名前を書く．
例）
チームA,チームAの1番目のレーサー,チームAの2番目のレーサー,チームAの3番目のレーサー
チームB,チームBの1番目のレーサー,チームBの2番目のレーサー,チームBの3番目のレーサー
チームC,チームCの1番目のレーサー,チームCの2番目のレーサー,チームCの3番目のレーサー
...



####キーボード操作
vimium等のプラグインは無効化しておいてください．

* zキー：レースが開始したとき，バトンパスしたとき，終了したとき

* aキー：リタイア宣言したとき

* cキー：結果を保存したいとき，result_state.csv（各チームのボーナス状況）

* result_time.csv（各セクションの時間の長さ）をダウンロード

  複数ファイルのダウンロードを許可してください．

* escキー：画面上でアクティブなチームの結果を削除

* xキー：間違ってzキーでバトンパスしてしまい，やり直したいとき
  ただし，aキーでリタイアしたときや，zキーでゴールしたときは復旧不可能なので注意！

* レース終了後
  ダウンロードしたresult_state.csvとresult_time.csvを，dataフォルダ下に置けば，レース結果の時間が復旧できる．
  ただし，各種ボーナスは内部変数で処理しているものの，復旧後の画面には反映されていないことに注意！