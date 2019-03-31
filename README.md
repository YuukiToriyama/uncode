# Uncode Manual
### ver. 2019/03/31

## 概要
ウンコードアプリは任意の文字列をうんこの羅列に変換し、暗号化します。
ウンコードはUnicodeの異字体セレクタを利用したアプリです。Unicodeには多数のカラー絵文字が収録されていますが、これらの絵文字に異字体セレクタ「U+FE0E」を付加してやると「対応したフォントがある環境下では」白黒の絵文字が表示されます。
そのため、白黒表示に対応したフォントがない環境下ではカラーのウンコも白黒のウンコもおなじ「💩」に映ります。
このことを利用した暗号化スクリプトです。
なお、スクリプト内の「環境設定」をいじれば💩ではなく🍎などでエンコードを行なうこともできます。

## Usage
./uncode.sh [ARGUMENT_1] [ARGUMENT_2]

## Example
$ ./uncode.sh "Hello, unko"

=> 💩︎💩💩💩︎💩💩💩💩💩︎💩︎💩💩💩︎💩💩︎💩💩︎💩︎💩💩︎💩︎💩💩💩💩︎💩︎💩💩︎💩︎💩💩💩💩︎💩︎💩💩︎💩︎💩︎💩︎💩💩💩︎💩💩︎💩︎💩💩💩💩︎💩︎💩︎💩💩︎💩💩︎💩💩︎💩︎💩💩︎💩︎💩︎💩💩💩︎💩︎💩💩︎💩💩︎💩︎💩💩︎💩︎💩💩︎💩︎💩︎💩︎💩💩💩💩💩︎💩💩︎💩

$ ./uncode.sh -d "💩︎💩💩💩︎💩💩💩💩💩︎💩︎💩💩💩︎💩💩︎💩💩︎💩︎💩💩︎💩︎💩💩💩💩︎💩︎💩💩︎💩︎💩💩💩💩︎💩︎💩💩︎💩︎💩︎💩︎💩💩💩︎💩💩︎💩︎💩💩💩💩︎💩︎💩︎💩💩︎💩💩︎💩💩︎💩︎💩💩︎💩︎💩︎💩💩💩︎💩︎💩💩︎💩💩︎💩︎💩💩︎💩︎💩💩︎💩︎💩︎💩︎💩💩💩💩💩︎💩💩︎💩"

=> Hello,unko

$ ./uncode.sh -h

=> このヘルプページが表示されます。


## (2019/03/31追記) rubyバージョンも作りました
```bash
echo "きょうも快調" | ruby uncode.rb
```
