# 公式チュートリアルを読みながらつくる Next.js

## Practice 01 プレーンなJavascriptでつくる動的なページ（命令型プログラミング）

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/updating-ui-with-javascript "")

htmlファイルに記述したDOMと、ブラウザに表示されるDOMが異なっているのが分かる。

これはhtmlファイルが最初のページコンテンツを表現するのに対して、DOMはDOMメソッドとjavascriptによって更新されたページコンテンツを表現しているから。

script要素の中に記述されている処理を見ると、純粋なjavascriptだけで1つの要素を追加するのに、5行もの処理が必要になるこことがわかる。

純粋なjavascriptだけでは、規模の大きなアプリケーションの開発には向かないことが分かる。

Practice 01 の方法を「命令型プログラミング」と呼ぶ。

## Practice 02 Reactを導入した動的なページ（宣言型プログラミング）

[参考サイト](https://nextjs.org/learn/foundations/from-javascript-to-react/getting-started-with-react "")

Reactを使えば、同じ処理でもプレーンなjsよりもコードを削減できる。

## Practice 03 Reactを導入した動的なページ（宣言型プログラミング）

Component は、関数の返り値としてUI要素を返すJavascriptの「関数」でしかない。

Component は、頭文字を大文字にしてHTMLやJavascriptと区別して扱う。

Component は、< /> で囲って使う。 ※ 関数名の時は< />はつかない。

Component は、それぞれお互いに入れ子にすることができるが、レンダリングのための最上位要素しか ReactDOM.render() には渡すことができない。

## Practice 04 Component は、複製して再利用することができる。

Component を複製して再利用すると、表示内容やスタイルなどすべて同じ要素が複製される。

## Practice 05

props を使うことで、Componentに引数を渡して、その引数を要素の中で使うことができる。

Props は、Component が動作する時や画面にレンダリングされた時の引数にできる。
