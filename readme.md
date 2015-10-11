# iro.Color.js

詳細なAPIドキュメントについては[api.md](api.md)をご覧ください。

**このライブラリはまだベーター段階です** 可能な限り、繰り返しのテストを行っていますが、期待しない結果が現れたり、設計上の問題がある可能性があります。お気づきの点はお気軽にご連絡いただけると幸いです。

## 直感的に色を操作できるライブラリです

iro.Color.jsを使えば直感的な記述で色を扱うことができます。

たとえば次のようにHSLとして初期化した色でも、そのままRGBやCMYKの色情報を取得・設定して、RGBの書式で出力したりといったことが可能です。

```javascript
var color = new iro.Color('hsla(228,80,32,1.0)');
color.r += 60.0; // 赤を60上げる
color.h += 20.0; // 色相を20度回転させる
color.k -= 10.0; // 黒を10落とす
document.getElementById('elem').style.color = color.css('rgb');
```

* RGB, CMYK, HSL, HSVの4種類のカラーモデルに対応しています ⇒ [a, r, g, b, h, s, v, l, c, m, y, k プロパティ](api.md#a-r-g-b-h-s-v-l-c-m-y-k-プロパティ)
* #FFFFFFなどのhex形式はもちろんrgb, hslなどの文字列形式からのインスタンス化、また再び文字列に戻すことが可能です ⇒ [コンストラクタ](api.md#コンストラクタ), [css メソッド](api.md#css-メソッド)
* ペイントソフトなどで用いられている色の合成（スクリーン、覆い焼き、オーバーレイなど）も可能です ⇒ [blend メソッド](api.md#blend-メソッド)

## あなたのページに追加しましょう

次のようなscriptタグをあなたのHTMLファイルに追加してください。

```html
<script type="text/javascript" src="iro.color.js"></script>
```

デバック情報が必要ない場合はminifiedバージョンをご利用下さい。
```html
<script type="text/javascript" src="iro.color.min.js"></script>
```

実行に必要なのは iro.color.js または iro.color.min.js のどちらか片方だけです。

iro.color.jsもしくは、iro.color.min.jsは、**必ずダウンロードして使用してください** 現在のところCDNは用意できておりません。直接的なリンクはいただけません。



## 商用・非商用問わず自由にご使用いただけます

iro.Color.jsおよびiro.Color.min.jsはMITライセンスにて提供します。

* 商用・非商用問わず誰でも無償で無制限にご利用いただけます。
* 著作権者はソフトウェアに関してなんら責任を負いません。

著作権は放棄していません。jsファイルに含まれる著作権表示を消してはいけません。

## 以下のブラウザで動作します

以下の表には検証が必要です。実際に確認はしておらず理論値に過ぎません。

ブラウザ          | バージョン
-----------------|-----------
Internet Explorer| ≧ 9
IE Mobile        | ≧ 9.0
Firefox (Gecko)  | ≧ 4.0
Firefox Mobile   | ≧ 4.0
Chrome           | ≧ 5
Safari           | ≧ 5.1
Opera            | ≧ 11.60
Opera Mobile     | ≧ 11.5



* * *

&copy; 2015 Retorillo
[twitter/retorilo](https://twitter.com/retorillo) 