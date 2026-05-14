# Base45QR

QRコードに適したBase45形式とバイナリデータ間のエンコードおよびデコードを行うライブラリです。

## デモ
https://code4fukui.github.io/Base45QR/

## 特徴
- バイナリデータをBase45形式にエンコード
- Base45形式をバイナリデータにデコード
- QRコードでの利用に最適

## 使い方
```js
import { Base45QR } from "https://code4fukui.github.io/Base45QR/Base45QR.js";

console.log(Base45QR.encode(new Uint8Array([ 15, 255, 79, 209, 104, 252 ])));
console.log(Base45QR.encode(new Uint8Array([ 218 ])));
console.log(Base45QR.decode("01234ABCD"));
console.log(Base45QR.decode("%4"));
```

## 参考
- [RFC 9285 - The Base45 Data Encoding (日本語訳)](https://tex2e.github.io/rfc-translater/html/rfc9285.html)

## ライセンス
MIT License — 詳細は [LICENSE](LICENSE) を参照してください。
