# Base45QR

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A library for encoding and decoding binary data to/from Base45 format, which is suitable for QR codes.

## Demo
https://code4fukui.github.io/Base45QR/

## Features
- Encode binary data to Base45 format
- Decode Base45 format to binary data
- Suitable for use in QR codes

## Usage
```js
import { Base45QR } from "https://code4fukui.github.io/Base45QR/Base45QR.js";

console.log(Base45QR.encode(new Uint8Array([ 15, 255, 79, 209, 104, 252 ])));
console.log(Base45QR.encode(new Uint8Array([ 218 ])));
console.log(Base45QR.decode("01234ABCD"));
console.log(Base45QR.decode("%4"));
```

## Reference
- [RFC 9285 - The Base45 Data Encoding (Japanese translation)](https://tex2e.github.io/rfc-translater/html/rfc9285.html)

## License
MIT License — see [LICENSE](LICENSE).