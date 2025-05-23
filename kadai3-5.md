## 自動販売機（データ構造と各種処理）のミニレポート
### Q5-1. 自動販売機の商品データついて説明せよ。
* データ構造（各項目とその説明）
id.name.priceなどといった連想配列の配列として定義されている。
* 連想配列の配列として定義するメリット
* メリットは拡張性である。新しい商品を追加する際、単に新しいオブジェクトを配列に追加するだけで済むため、データ構造が柔軟で拡張しやすくなる。
### Q5-2. showItemListの処理内容について説明せよ。
* 配列の繰り返し処理
*  showItemList関数ではforを使用して配列内の各商品オブジェクトを繰り返し処理している。
* 連想配列の参照方法
* item.id,item.name.item.priceなどのようにドット記法を用いてプロパティにアクセスしています。
### Q5-3. buyItemの処理内容について説明せよ。
* 商品購入の可否判定
* buyItem関数は因数として受け取ったた商品番号が1からitems.lengthの範囲内にあるかを確認する。範囲外の場合はエラーメッセージを表示し、処理を終了しこの判定により、無効な商品番号によるエラーを防いでいる。
* 商品在庫を減らす処理
* 有効な商品番号が指定された場合、item.stockをチェックし、在庫がある場合はその商品の在庫数を1減らす。これにより、購入処理が正常に行われたことを示している。
* 商品番号のエラー処理
* エラー処理は○○については無効な番号であり正しい指定をしてくださいという表示をされる。
### Q5-4. プログラムの考察
* データ構造について
* 商品情報はオブジェクトの配列として表現されているためこのデータ構造により商品情報の管理が容易になると思っている。
* 商品一覧表示と購入処理を関数化したメリット
* メリットとして再利用性である。
* 関数化することにより同じ処理を何度も呼び出すことができコードの重複を避けることができる。
### Q5-5. 感想
* 今回の課題で苦労したこと
* 課題４のプログラミングが苦労した
* 演習を通して理解できたこと
* １限目で習ったような事を理解できた。
* この自動販売機プログラムの追加機能や課題など
* 今はまだ理解していない部分が多々あるのでその復習からしていこうと思っている。
